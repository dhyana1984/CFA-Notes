# Probability Distribution
## Discrete Random Variable 离散随机变量
* 有限的，或者可数的（抛骰子，进银行办业务的人数）


## Continuous Random Variable 连续随机变量
* 无限且不可数，某地区降雨量
* 通常取值在某一区间内，即使存在上下界，仍然有无穷多个
* 每一点的概率为0，但是概率为0是个数学概念，不等于不可能发生
* 在研究一些问题时可以把离散变量近似看成是连续随机变量

## Distribution Function 分布函数
### Probability Density Function PDF 概率密度函数
* 对某个随机变量所有可能取值及对应概率进行描述的函数
* PDF用f(x)表示，函数图像与x轴区间$[x_1,x_2]$围城的面积即为随机变量X在区间$[x_1,x_2]$内的概率，实际上就是f(x)在$[x_1,x_2]$上的定积分$\int_{x_1}^{x_2}f(x)\,\rm{d}x$
* PDF f(x)非负，并且与x轴围成的面积为1
* 由于连续随机变量取任意一点概率为0，所以开区间闭区间无所谓
  
### Cumulative Distribution Function CDF 累积分布函数
* 代表累积的概率，即随机变量X小于某特定值x的概率，通常记为$F(x)=P(X\leq{x})$
* CDF是有界的
  $$F(-\infty)=P(X\leq-\infty) =0$$
  $$F(+\infty)=P(X\leq+\infty) =1$$
* 累积分布函数时单调递增的，$若x_1\leq x_2，F(x_1)\leq F(x_2)$
* $P(x_1\lt X \leq x_2) = P(X\leq x_2)-P(X\leq x_1) = F(x_2)-F(x_1)$
* 离散随机变量的累积分布函数呈现出阶梯状
* 连续型PDF f(x)与CDF F(x)关系，F(x)的取值实际上就是f(x)函数与区间$[-\infty, x]$围城的面积

## Discrete Distribution 离散分布
### Discrete Uniform Distribution 离散均匀分布，每个取值对应概率是相等的，即均匀的
### Bernoulli Distribution 伯努利分布，伯努利分布又称为两点分布，指随机变量X只有可能取值结果1与0
### Binomial Random Variable 二项分布
二项分布就是度量进行n此伯努利实验，成功次数为X=x的概率(x为0到n之间的任意整数)
$$B(n,p)，n与p为二项分布的两个参数，不同次实验是相互独立的，每次试验成功概率为常数p$$
定义随机变量X为n次伯努利实验中的成功次数，每次成功概率为p，则P(X=x)的概率为：
$$P(x)=C_n^xp^x(1-p)^{n-x}=\frac{n!}{(n-x)!x!}\,p^x(1-p)^{n-x}$$

## 连续分布
### Continuous Uniform Distribution 连续均匀分布
* 连续均匀分布每一个单点的概率都等于0，均匀是针对**区间**而言，而不是单个点
* 连续均匀分布的概率密度函数 PDF，对于任意随机变量X区间$[x_1,x_2]$的PDF
$$
f(x) = 
  \left\{
      \begin{aligned}
           \frac{1}{b-a} & & (a\leq x \leq b) \\
           \\
           \text{0} & & (otherwise)
      \end{aligned}
 \right.
$$
* 随机变量X在$[x_1,x_2]$区间的概率为区间$[x_1,x_2]$与PDF围城的面积，即长为(x_2-x_1)，高为$\frac{1}{b-a}$的矩形面积
$$
    P(x_1 \leq X \leq x_2) = \frac{X_2-x_1}{b-a}
$$
* 连续均匀分布的 CDF
$$
f(x) = 
  \left\{
      \begin{aligned}
           0 && (x \leq a) \\
           \\
           \frac{x-a}{b-a} & & (a\lt x \lt b) \\
           \\
           1 & & (x \geq b)
      \end{aligned}
 \right.
$$

