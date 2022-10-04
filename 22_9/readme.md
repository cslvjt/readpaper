# DASR
[Efficient and Degradation-Adaptive Network for Real-World Image Super-Resolution](https://arxiv.org/abs/2203.14216)

## 贡献及解决难点
+ 作者提出一种高效且有用的degradation-adaptive super-resolution(DASR)，该网络大致可以分为两部分：一个微小的回归网络被用来预测输入图像的退化参数，几个具有相同拓扑的convolutional experts联合优化，通过experts的非线性混合来指定网络参数。

# ELAN
[Efficient Long-Range Attention Network for Image Super-resolution](https://arxiv.org/abs/2203.06697)

## 贡献及解决难点
+ 应用accelerated self-attention(ASA)组成group-wise multi-scale self-attention(GMSA)。GMSA和shift-conv组成ELAB。ELAB堆叠组成ELAN。
+ 一种轻量化的超分网络。