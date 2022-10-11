# EDSR
[Enhanced Deep Residual Networks for Single Image Super-Resolution](https://arxiv.org/abs/1707.02921)
## 作者贡献
+ 作者通过消除传统残差网络中无用的模块提升性能。即去除batchnormal
+ 提出一个新的多阶段结构能够在不同尺度上共享参数。即在X2尺度上的参数初始化X3、X4尺度