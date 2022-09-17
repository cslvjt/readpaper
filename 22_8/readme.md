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
+ [MLP-Mixer](MLP_Mixer/introduction.ipynb)

## MAXIM
[MAXIM: Multi-Axis MLP for Image Processing](https://arxiv.org/pdf/2201.02973v2.pdf)
### 贡献及解决的难点
两个新的模块，组成的多阶段多尺度模型
+ Maxim的关键设计是使用多轴方法并行捕获本地和全局交互信息。通过在每个分支的单个轴上混合信息，该基于MLP的操作变为“fully-convolutional”，并且相对于图像大小线性缩放，这大大提高了其对密集图像处理任务的灵活性。(sec 3.2)
+ 针对低级视觉任务量身定制的多轴门控MLP模块，该模块始终享有全局感受野，和图像尺寸呈线性相关。
+ 作者还定义并构建了一个基于MLP的纯交叉门控模块，该模块可以使用相同的多轴方法适应gate the skip-connections in the neck of MAXIM，并进一步提高性能。(sec 3.3)
+ [MAXIM code](MAXIM/introduction.ipynb)