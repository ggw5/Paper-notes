# **PDL: A Data Layout towards Fast Failure Recovery for Erasure-coded Distributed Storage Systems**

## 背景

纠删码的修复：沉重的跨机架修复流量以及不均匀的跨机架修复流量 

## 技术方法

PDL：平均的在集群中放置条带的块

rPDL：基于PDL的修复方法

1. 选择替换节点：

如果存在未满rack（<m）则选择其中的节点

如果不存在未满rack则随机选择一个和当前条带无关的rack

2. 选择幸存的块来恢复丢失的块：
    按照PDL来放置块的话，每个和当前条带有关的rack都会参与修复（除了存放失效节点的rack）

3. 解码方案：

现在机架中做聚集修复，然后跨机架传送部分修复块，以此来减少跨机架流量

## 实验环境

testbed，集成HDFS

## 指标

跨机架修复流量，修复吞吐量，降级读延迟

 

 