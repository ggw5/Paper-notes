# **Fast Erasure Coding for Data Storage: A Comprehensive Study of the Acceleration Techniques**

## 背景

将独立的加速编码的方法结合起来（使用bitmatrix的方法） 

## 技术方法

1.遗传算法的到优化后的bitmatrix；

2.进行归一化（bitmatrix normalization）；

3.使用UM（Unweighted matching）或WM（Weighted matching）找到common XOR chains；

4.cache优化，Ⅰ：data bit->parity bit/中间结果bit；Ⅱ：中间结果bit->parity bit。减少cache miss

5.向量化异或操作（CPU单指令多数据SIMD性质）

## 实验

testbed

## 指标

编码和解码吞吐量