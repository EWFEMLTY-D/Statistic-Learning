#  统计学习方法

##  第一章 统计学习概况

###  1. 统计学习分类

>  统计学习包括监督学习、非监督学习、半监督学习及强化学习

![](https://i.bmp.ovh/imgs/2022/01/733c706d13055a75.png)

###  2. 统计学习方法三要素

####  2.1 监督学习

##### 2.1.1 模型

> 在监督学习过程中，模型就是所要学习的条件概率分布或决策函数。模型的假设空间（hypothesis space）包含所有可能的条件概率分布或决策函数。假设空间中的模型一般有无穷多个

##### 2.1.2 策略

> 损失函数度量模型一次预测的好坏，风险函数度量平均意义下模型预测的好坏

> 0-1 损失函数主要针对分类问题，平方损失函数&绝对损失函数主要针对回归问题，对数损失函数：主要针对概率模型

![](https://s3.bmp.ovh/imgs/2022/01/5d75af893e6d4c7e.png)

> 模型训练的终极目的是为了降低期望风险，但由于联合分布 P(X, Y) 是未知的，所以期望风险只存在理论意义。根据大数定律，当样本容量 N 趋于无穷时，经验风险趋于期望风险。因此，在实际训练时，我们可以用经验风险去近似期望风险

> 针对样本容量大小，存在两种训练策略：经验风险最小策略和结构风险最小策略；当样本容量足够大时，经验风险最小策略就能保证较好的训练效果；如果训练样本有限，经验风险最小策略就会产生“过拟合”，可在经验风险的基础上增加表示模型复杂度的正则化项（罚项），即结构风险最小策略（Structural Risk Minimization, SRM）

![](https://i.bmp.ovh/imgs/2022/01/e0cbf6530bc921b5.png)

##### 2.1.3 算法

> 用于求解最优模型

#### 2.2 无监督学习

![](https://s3.bmp.ovh/imgs/2022/01/332b7bd3e4df9f8a.png)

##  第二章 感知机

###  1. 模型介绍

![](https://s3.bmp.ovh/imgs/2022/01/b0be3c47628ec25d.png)

###  2. 学习策略

> 找出点到超平面的距离公式，损失函数就是所有误分类点到超平面的和，范数||w||对损失函数的值不影响，所以去掉

![](https://s3.bmp.ovh/imgs/2022/01/952ea5e0d7939a0e.png)

![](https://s3.bmp.ovh/imgs/2022/01/0e788f0a675640a6.png)

###  3. 梯度下降法

![](https://s3.bmp.ovh/imgs/2022/01/c9b4f18d9dedeb79.png)

###  4. 原始形式算法



###  5. 对偶形式算法



