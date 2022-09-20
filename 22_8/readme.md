## gMLP
[pay attention to mlps](http://arxiv.org/abs/2105.08050)
### 贡献及解决的难点
+ 作者提出一种新的基于MLP的网络结构，gMLP。性能和transformer一样优异，不管是在NLP还是CV
+ [gMLP code](gMLP/introduction.ipynb)
## MLP-MIXer
[MLP-Mixer: An all-MLP Architecture for Vision](http://arxiv.org/abs/2105.01601)
### 贡献及解决的难点
+ 提出使用简单的mlp达到SOTA
+ 提出token-mix，channel-mix结构
+ [MLP-Mixer code](MLP_Mixer/introduction.ipynb)

## MAXIM
[MAXIM: Multi-Axis MLP for Image Processing](https://arxiv.org/pdf/2201.02973v2.pdf)
### 贡献及解决的难点
两个新的模块，组成的多阶段多尺度模型
+ Maxim的关键设计是使用多轴方法并行捕获本地和全局交互信息。通过在每个分支的单个轴上混合信息，该基于MLP的操作变为“fully-convolutional”，并且相对于图像大小线性缩放，这大大提高了其对密集图像处理任务的灵活性。(sec 3.2)
+ 针对低级视觉任务量身定制的多轴门控MLP模块，该模块始终享有全局感受野，和图像尺寸呈线性相关。
+ 作者还定义并构建了一个基于MLP的纯交叉门控模块，该模块可以使用相同的多轴方法适应gate the skip-connections in the neck of MAXIM，并进一步提高性能。(sec 3.3)
+ [MAXIM code](MAXIM/introduction.ipynb)

## NAFNet
[Simple Baselines for Image Restoration](http://arxiv.org/abs/2204.04676)
### 所做的贡献以及解决的问题
+ 提出一个新的图像恢复领域的baseline，SOTA
+ 通过用数学的方式或者直接去除，搭建一个无激活函数的网络
+ 块内复杂性和块间复杂性的概念（related work）
+ [NAFNet code](NAFNet/introduction.ipynb)

## RGIA
[Improving Image Restoration by Revisiting Global Information Aggregation](http://arxiv.org/abs/2112.04491)
### 所做的贡献以及解决的问题
+ 第一个提出基于patch训练和基于全图像测试中统计分布的变化可能会导致性能下降
+ 为了实际减少训练和测试之间的统计分布变化，作者分析了现有方法的缺点，并提出了TLC,以弥合训练和推理之间的信息聚合差距。全局操作（例如，SE模块中的全球平均池[13]中的全局平均池）仅在推理期间转换为局部操作，因此它们像训练阶段一样在本地空间区域内汇总特征。因此推理期间的整个基于图像的“本地”信息具有与基于补丁的“全局”信息分布相似。TLC在不进行重新训练或微调的情况下，取代了从全局到局部的统计汇总操作，通过减少训练测试不一致大大提高性能
+ [code](RGIA/introduction.ipynb)