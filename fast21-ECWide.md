# **Exploiting Combined Locality for Wide-Stripe Erasure Coding in Distributed Storage**

## 背景

大纠删码极度压缩冗余，但是因此增大其他方面的开销（修复，编码），尤其是修复开销，为了减少修复开销提出了Combined Locality方法。

## 技术方法

修复：结合两种locality：parity locality和 topology locality来产生最小的跨机架修复流量

全节点修复时选择LRC来选择不同的节点进行重构，从而并行修复

编码：将k分为小的子任务给其他节点，每个节点计算出部分校验块，最后汇合成完整校验块

更新：全局校验更新：只传data delta

局部校验更新：让局部校验块和更新频率最高的数据块放在一个机架内

## 实验环境

testbed

## 指标

以时间为指标测试修复、编码和更新性能