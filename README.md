# 1. 机器学习

## 1.1. postive and unlabeled data问题

* [conversion delay](http://www0.cs.ucl.ac.uk/staff/w.zhang/rtb-papers/delayed-feedback.pdf)使得negative label不一定真的是negative的，论文通过对conversion delay建模，提出的DFM(Delayed Feedback Model)模型可以理论上获得更准的cvr预估结果，而且可以使用SGD算法求解，实用性很强。

## 1.2. position bias问题

* 2012年微软的paper[Position-Normalized Click Prediction in Search Advertising](https://pdfs.semanticscholar.org/5c53/c7101b530eae80417beeba16684d789056f2.pdf), 从用户终端收集到的数据，一方面好广告的位置更加靠前，而好位置的ctr又天然偏高，而这个在数据上是耦合在一起的。论文提出factor model对位置和广告相关性分开建模，通过模拟数据验证理论上可以得到更加准确的ctr预估结果。

## 1.3 tree model

* 经久不衰的GBDT模型，目前效果最好的[LightGBM](http://www.msra.cn/zh-cn/news/blogs/2017/01/lightgbm-20170105.aspx)，LightGBM[优化方法](http://www.msra.cn/zh-cn/news/blogs/2017/01/lightgbm-20170105.aspx)。

## 1.4 unbalanced classes问题

* [Learning from Imbalanced Classes](https://www.svds.com/learning-imbalanced-classes/)，文章指出的bagging方法可能会有一些帮助。

# 2. 推荐算法

## 2.1 矩阵分解

* Koren在2009年提出的[Matrix Factorization模型](https://datajobs.com/data-science-repo/Recommender-Systems-%5BNetflix%5D.pdf)相比于协同过滤CF算法，具有三个优势：1）更容易引入更多信号；2）可扩展性强，也就是可并行化学习；3）准确率比CF更高。几个boosting的tricks：1）with bias，2）通过引入implicit feedback改进explicit feedback效果，这在目标数据稀疏的情况下会卓有成效，3）考虑时间因素，2012年Koren公开了如何考虑时间因素的[paper](https://pdfs.semanticscholar.org/8451/c2812a1476d3e13f2a509139322cc0adb1a2.pdf)，但是有点晦涩，没有仔细看，实际工业应用中，该环节是非常重要的一个feature，待回头仔细研究。

# 3. 强化学习

* David Silver的[DPG算法](http://proceedings.mlr.press/v32/silver14.pdf),
* David Silver的[DDPG算法](https://arxiv.org/pdf/1509.02971v2.pdf)
* 使用target network[Human-level control through deep reinforcement learning](http://www.cdf.toronto.edu/~csc2542h/fall/material/csc2542f16_dqn.pdf)
* 使用tensorflow实现[DDPG算法](Deep Deterministic Policy Gradients in TensorFlow]

# 4. 面试

## 4.1 如何面试深度学习候选人

* [如果你是面试官，你怎么去判断一个面试者的深度学习水平？](https://www.zhihu.com/question/41233373)


# 5. 基础知识

## 5.1 数学基础知识

* [【官方双语/合集】线性代数的本质 - 系列合集](http://www.bilibili.com/video/av6731067/)
* [【官方双语】微积分的本质](http://www.bilibili.com/video/av10308208/)

# 6. 演讲材料

## 6.1 ppt制作素材

* pinterest.com
* 免费高清图库https://visualhunt.com/,http://www.gratisography.com/

