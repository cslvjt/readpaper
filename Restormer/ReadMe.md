# 文件夹介绍
图像恢复领域相关的论文
## MPRNet
https://ieeexplore.ieee.org/document/9577298/
### 所做的贡献以及解决的问题
+ 提出一个多阶段模型，将图像恢复任务分解为多项子任务。SOTA
+ 一个有效的监督注意力模块，在进一步传播之前，在优化传入特征的每个阶段都充分利用恢复的图像。
+ 一种融合多尺度特征信息的策略(CSFF)
+ [MPRNet code](MPRNet/MPRNet.ipynb)
## MIMO-UNet
http://arxiv.org/abs/2108.05054
### 所做的贡献以及解决的问题
+ 新的以coarse-to-fine方式去模糊
+ 类UNet架构，简单但有效
+ 采用的非对称特征融合在多阶段中很有用
+ [MIMO-UNet code](MIMO-UNet/MIMO-UNet.ipynb)
## SDWNet
https://ieeexplore.ieee.org/document/9607841/
### 所做的贡献以及解决的问题
+ 在图像去模糊中使用小波变换和扩张卷积
+ 单阶段模型，易训练
+ [SDWNet code](SDWNet/SDWNet.ipynb) 
## Restormer
https://arxiv.org/abs/2111.09881
### 所做的贡献以及解决的问题
+ 将transformer应用到图像恢复领域
+ 将QKV在通道维度应用，这样复杂度是线性的
+ 采用一种新的训练方式：渐进式训练。在早期epoch中，使用小patch大batch，然后逐渐改变为大patch小batch
+ 新的block：GDFN和MDTA
+ [Restormer code](Restormer/introduction.ipynb)
## NAFNet
http://arxiv.org/abs/2204.04676
### 所做的贡献以及解决的问题
+ 提出一个新的图像恢复领域的baseline，SOTA
+ 通过用数学的方式或者直接去除，搭建一个无激活函数的网络
+ 块内复杂性和块间复杂性的概念（related work）
+ [NAFNet code](NAFNet/introduction.ipynb)
## Improving Image Restoration by Revisiting Global Information Aggregation
http://arxiv.org/abs/2112.04491
### 所做的贡献以及解决的问题
+ 第一个提出基于patch训练和基于全图像测试中统计分布的变化可能会导致性能下降
+ 为了实际减少训练和测试之间的统计分布变化，作者分析了现有方法的缺点，并提出了TLC,以弥合训练和推理之间的信息聚合差距。全局操作（例如，SE模块中的全球平均池[13]中的全局平均池）仅在推理期间转换为局部操作，因此它们像训练阶段一样在本地空间区域内汇总特征。因此推理期间的整个基于图像的“本地”信息具有与基于补丁的“全局”信息分布相似。TLC在不进行重新训练或微调的情况下，取代了从全局到局部的统计汇总操作，通过减少训练测试不一致大大提高性能
+ [code](RGIA/introduction.ipynb)