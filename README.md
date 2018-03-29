关于大数据的一些基本概念。

HDFS:  Namenode : 存储 fsimage 和 edits ,并在内存中维持每个block块的datanode的映射关系。 Datanode： 会向namenode发送最新block的信息。
       SNamenode： 定期对namenode的Fsimage 和edit 做merge，并返回给namenode。因此需要的内存和namenode 差不多。
       HA: 
