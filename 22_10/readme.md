# EDSR
[Enhanced Deep Residual Networks for Single Image Super-Resolution](https://arxiv.org/abs/1707.02921)
## 作者贡献
+ 作者通过消除传统残差网络中无用的模块提升性能。即去除batchnormal
+ 提出一个新的多阶段结构能够在不同尺度上共享参数。即在X2尺度上的参数初始化X3、X4尺度
# shiftNet
[Shift: A Zero FLOP, Zero Parameter Alternative to Spatial Convolutions](https://openaccess.thecvf.com/content_cvpr_2018/papers/Wu_Shift_A_Zero_CVPR_2018_paper.pdf)
## 作者贡献
+ 作者提出一种新的卷积方式命名为shiftConv，该卷积可以减轻模型的参数
+ 深度可分离卷积大部分时间用来访问内存，限制并行硬件的使用。而shiftConv则减轻这一问题。
+ shiftConv可以和模型剪枝、模型压缩等方法一起使用。