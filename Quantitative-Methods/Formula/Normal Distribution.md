# Normal Distribution 正态分布
* 正态分布的PDF可由均值和方差完全刻画，记为$N(μ,\sigma^2)$
* 根据PDF图形，在均值μ附近的取值概率较大，极大极小值概率比较小
* 正态分布的偏度为0，峰度为3
* 服从正态分布且相互独立的随机变量的线性组合也服从正态分布，如果随机变量X和随机变量Y服从正态分布，aX+bY也服从正态分布
* 如果随机变量X服从正态分布，则
  * X落在$[\mu-\sigma,\mu+\sigma]$的概率为**68%**
  * X落在$[\mu-1.65\sigma,\mu+1.65\sigma]$的概率为**90%**
  * X落在$[\mu-1.96\sigma,\mu+1.96\sigma]$的概率为**95%**
  * X落在$[\mu-2.58\sigma,\mu+2.58\sigma]$的概率为**99%**

## Standard normal distribution 标准正态分布
均值为0，方差为1的正态分布即为standard normal distribution标准正态分布，通常称之为Z分布，
$$
P(X\leq x) = P(\frac{X-\mu}{\sigma}\leq \frac{x-\mu}{\sigma})=\Phi(\frac{x-\mu}{\sigma})
$$
$\Phi(x)$就是标准正态分布的CDF，利用$\frac{X-\mu}{\sigma}$得到的值称为z值，求z值的过程就是标准化，把$\sigma$看成是PDF途中横轴单位，z值描述的就是随机变量X距离其均值的距离

## 亏空风险
* 假设资产收益率服从正态分布，那么收益率的方差就衡量了资产收益率变动的风险，用方差来衡量风险主要是强调收益率的不确定性，包括收益率低于均值情况，也包括高于均值情况。
* 想单独考查收益率低于某个特定水平的风险，就要引入shortfall risk 亏空风险，亏空风险是指资产收益率在一段时间内低于最低可接受水平$R_L$(minimum acceptable level, 也称为shortfall Level)的概率。
* 亏空风险是一个**概率**

## Roy's Safety-First Ratio
投资者通过最大化罗伊安全第一比例来实现最小化亏空风险$P(R<R_L)$，Roy's Safety-First Ratio as below
$$
SF_{ratio} = \frac{E(R_p)-R_L}{\sigma_p}，R_L= Shortfall\;Level，E(R_p)=资产p的收益率，\sigma_p=标准差 \\
当R_L=R_F无风险收益率时，此公式结果就是求夏普比率
$$
**最大化第一安全比例就是最小化亏空风险，两者等价**

## 对数正态分布
* 对数正态分布的概率密度函数是非负的
* 对数正态分布的概率密度函数是正偏的
* 对数正态分布是用来衡量资产价格的，而正态分布主要用来衡量收益率
* 已知随机变量$X$服从正态分布，则$e^X$服从对数正态分布，因为$\ln{e^x}=X$服从正态分布

## Student's t-Distribution 学生t分布
* t分布的PDF可以由一个参数完全刻画，degress of freedom df自由度，通常记为t(n)，n代表自由度，为正整数
* t分布的PDF也是一条钟形曲线，左右对称，尾部比正太分布要厚，偏度=0，峰度>3
* 当t分布的自由度趋近于无穷大时，t分布的PDF会无限趋近于标准正态分布的PDF

