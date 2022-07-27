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

## Revisiting Global_Statistics_Aggregation