# **On the Optimal Repair-Scaling Trade-off in Locally Repairable Codes**

## 背景

在集群且使用LRC的场景下，权衡修复流量和扩展流量（跨集群） 

## 技术方法

构造最小扩展流量的布局opt-s，此时修复流量最大，一步步从core cluster中拿出local parity放到对于local data set所在集群中来减少修复流量（会增大扩展流量），最后会达到最小修复流量的布局opt-r。根据需要选择这个过程中的布局。

## 实验

数值分析和testbed

## 指标

扩展开销（扩容和缩容），修复开销

   时间