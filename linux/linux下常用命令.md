**常用指令**

  * 批量解压缩日志文件 ''find INFO_.log201*.bz2 | xargs -i tar jxvf {}''
  * 查看数 ''grep -rn "queryID" INFO_.log20* | grep "runBack" | wc -l''
  * GDB方式启动行云
      <code>
      将启动脚本中的$XCLOUD_BASE/bin/xcloudd $para 1>>LOG_.std_out_err 2>&1 &去掉，
      并替换为gdb --args $XCLOUD_BASE/bin/xcloudd $para 1
      </code>