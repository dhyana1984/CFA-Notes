# Probability
## Odds 赔率
* Odds for the Event E = $\frac{P(E)}{1-P(E)}$
* Odds aginst the Event E =$\frac{1-P(E)}{P(E)}$ 

## Probability Calculation

### 联合概率是指一组事件同时发生的概率，P(AB)
$$P(AB) = P(A|B)P(B)$$

### 条件概率的表达式为P(A|B)，本质上仍然是事件A的概率，只不过是估算事件B发生后事件A的概率，相当于原先的样本空间发生了变化，事件B为判断事件A的发生概率剔除了一些样本点
$$P(A|B) = \frac{P(AB)}{P(B)}$$
Tips: 一般if, given开头的句子，给出的是条件概率，而如果是以and连接两个事件，则一般给出的是联合概率

### 加法规则适用于求事件A或者事件B的发生概率，记为P(A or B)或者P(A+B)，只要A或B一个发生，则代表A or B发生
$$P(A or B) = P(A)+P(B)-P(AB)$$

### 全概率公式
$$P(B) = \sum_{i=1}^{N}P(A_i)P(B|A_i)，其中事件A_1,A_2...A_n互斥且遍历$$

### 贝叶斯公式
$$P(A|B) = \frac{P(B|A)}{P(B)}\times{P(A)}$$

### 相关系数
* 由于除以各自资产的标准差，相关系数的取值在-1到+1之间，当相关系数为1时，称为完全正相关(perfect positive correlation)，表示资产之间存在斜率为正的线性关系
* 相关系数为-1时，称为完全负相关(perfect negative correlation)，表示资产之间存在斜率为负的线性关系
* 只要相关系数绝对值为1，则资产之间存在线性关系
* scatterplot 散点图，相关系数越搞意味着资产线性关系越强，没有完全线性关系
* 相关系数为0只能说明没有线性关系，但是不能说明没有其他非线性关系

## Combination 组合
### 多项式公式， 将n个物品分为k类，即k个标签，第一类有$n_1$个物品，第二类有$n_2$个物品，第k类有$n_k$个物品，$n_1+n+2+...n_k = n$，分法有几种
$$C =\frac{n!}{n_1!n_2!{\ldots}n_k}$$

### 组合就是多项式公式的特立，将物品归为两类，r个物品一类，n-r个物品另一类
$$ C_n^r=\frac{n!}{(n-r)!r!}$$

### Permutation 排列
$$P_n^r = \frac{n!}{(n-r)!}$$