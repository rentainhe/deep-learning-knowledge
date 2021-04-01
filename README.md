# cv-interview
A collection of cv-interview problems and answers

## Contents
### 1. Coding
- [C++学习视频](https://www.bilibili.com/video/BV1et411b73Z?from=search&seid=18167644560005164073)
  - [搭配的学习笔记](https://blog.csdn.net/ClaireSy/article/details/108422945) 

### 2. Basic Knowledge

### 1. Image Classification

|    link    |summarization|
| :-----------: | --- |
|[交叉熵你真的懂了吗？](https://zhuanlan.zhihu.com/p/61944055)<br>[为什么分类任务使用交叉熵？](https://zhuanlan.zhihu.com/p/104130889)| 如果把分类任务看成回归问题, 回归问题往往需要使用sigmoid函数, 在求导反向传播时, 其导数会包含sigmoid的导数, 当其输出接近0和1的时候其导数非常小, 并且W和b的导数与sigmoid导数成正相关, 输出接近0和1的时候学习率非常小, 如果使用交叉熵的话则求导结果为sigmoid的值和label之差，误差越大其W和b的导数越大, 学习的也更快|
