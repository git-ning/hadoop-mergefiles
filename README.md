# HDFS合并小文件工具

## 功能

 合并集群中目录下的小文件

## 使用说明

` hadoop jar mergefiles.jar -h `

功能: 合并HDFS一个目录下的小文件，默认小于128M将被合并

版本:1.6

Usage: hadoop jar MergeTask -p 准备合并的HDFS全路径

高级参数说明：

        -p      指定准备合并的HDFS全路径,多个以逗号分隔，必选

        -s      设置小于size大小的文件将被合并，默认:128M

        -m      设置合并每个reducer处理的大小，默认:250M

        -n      是否递归合并，默认:递归合并

        -t      是否把不识别的文件认为是文本类型，默认:否

        -o      设置合并后输出的HDFS路径，默认:输入目录

        -f      指定一个本地文件作为输入合并目录

        -j      指定最大并行的job数

        -d      指定合并临时目录

        -u      指定文件格式(orc,lzo,text,avro等)

        -x      指定一个文件,内容为不需要合并的目录

        -l      计算目录起用的最大线程数.

