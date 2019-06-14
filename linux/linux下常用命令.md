**常用指令**

  * 批量解压缩日志文件 <code>find INFO_.log201*.bz2 | xargs -i tar jxvf {}</code>
  * 查看数 <code>grep -rn "queryID" INFO_.log20* | grep "runBack" | wc -l</code>
  * 截取日志中某部分内容并排序
    <code>
    grep -rn "queryID" INFO_.log20* | grep "runBack" | awk -F ' ' { 'print $5}' } | sort
    </code>
  * GDB方式启动行云
      <code>
      将启动脚本中的$XCLOUD_BASE/bin/xcloudd $para 1>>LOG_.std_out_err 2>&1 &去掉，
      并替换为gdb --args $XCLOUD_BASE/bin/xcloudd $para 1
      </code>