# cv-interview
A collection of cv-interview problems and answers

## Contents
### 1. Coding
- [C++学习视频](https://www.bilibili.com/video/BV1et411b73Z?from=search&seid=18167644560005164073)
  - [搭配的学习笔记](https://blog.csdn.net/ClaireSy/article/details/108422945) 
- __python基础知识github__
  - [python-interviews](https://github.com/revotu/python-interviews)
- __算法刷题优质github__
  - [algorithm-base](https://github.com/chefyuan/algorithm-base)

### 2. Basic Knowledge

|    link    | summarization |
| :---: | :--- |
| [1. 交叉熵你真的懂了吗？](https://zhuanlan.zhihu.com/p/61944055) <br> [2. 为什么分类任务使用交叉熵？](https://zhuanlan.zhihu.com/p/104130889) | 如果把分类任务看成回归问题, 回归问题往往需要使用sigmoid函数, 在求导反向传播时导数很小, 梯度更新很慢|
| [1. 为什么说随机最速下降法(SGD)是一个很好的方法？](https://zhuanlan.zhihu.com/p/27609238)<br>[ 2.【优化器】优化器算法及PyTorch实现（一）：永不磨灭的SGD ](https://zhuanlan.zhihu.com/p/77503211)<br>[3. 详解梯度下降法的三种形式BGD、SGD以及MBGD](https://zhuanlan.zhihu.com/p/25765735)<br>[4. 一个框架看懂优化算法之异同SGD/AdaGrad/Adam](https://zhuanlan.zhihu.com/p/32230623) | BGD: 批量梯度更新，每次用到了所有的数据的平均梯度，更新缓慢<br>SGD：每次更新只取一个样本，引入过多的噪声，优化不稳定<br>MBGD：将每一个batch作为一个样本，取平均Loss、梯度，进行梯度更新，缓解了SGD的优化不稳定问题，同时也减缓了GD的更新缓慢问题，减少参数更新次数，更新更加稳定，同时可以充分利用GPU并行计算，提高计算效率<br>无特殊说明的话，SGD优化器指的就是MBGD  |
| [1. Why Momentum Really Works](https://distill.pub/2017/momentum/)<br>[2. 深度学习最全优化方法总结比较](https://zhuanlan.zhihu.com/p/22252270)| 解释了SGD优化器中动量的作用，有利于逃出局部最小，并且对其进行了可视化<br>AdaGrad引入了对学习率的调整，在一定的学习积累后，后续的学习可能不需要特别大的学习率<br>Adam将SGD和AdaGrad的优点都结合起来 |
| [如何选择模型训练的batch size和learning rate](https://zhuanlan.zhihu.com/p/363645881) | 大的batch size在优化过程中更加稳定，但是泛化性能未必会好，因为容易落入鞍点，小的batch size优化过程不会很稳定，但是引入的噪声却有助于跳出鞍点，使得模型泛化能力更强 |
| [大小为1的卷积核有什么好处？](https://www.zhihu.com/question/56024942) | 有以下4个方面的好处：1. 降维（减少参数） 2.升维（用最少的参数来拓展维度） 3.跨通道信息交互，实现降维和升维的操作其实是channel间信息的线性组合变化，可以增强通道间信息的交互。 4.增加非线性特性，在大小为1的卷积后往往会加入激活层，可以在保持分辨率不变的情况下大幅增加非线性特性，将网络变得更加deep
