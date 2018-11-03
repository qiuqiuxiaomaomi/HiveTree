# HiveTree
Hive技术研究

![](https://i.imgur.com/HDhqsSZ.png)

<pre>
所有的命令和查询都会进入到Driver，通过该模块对输入进行解析编译，对需求的计算进行优化，然后按照指定的步骤执行(通常是启动多个MapReduce任务来执行)，当需要启动MapReduce任务时，Hive本身是不会生成Java MapReduce算法程序的，相反，Hive通过一个表示Job执行计划的XML文件驱动执行内置的，原生的Mapper和Reducer模块。

Hive通过和JobTracker通信来初始化MapReduce任务，而不必部署在JobTracker所在的管理节点上执行，在大型集群中，通常会有网关机专门用于部署像Hive这样的工具，

metastore(元数据存储)是一个独立的关系型数据库，Hive会在其中保存表模式和其他系统元数据。
</pre>

<pre>
安装环境
     Hive依赖于Hadooop，而Hadoop依赖于Java

</pre>