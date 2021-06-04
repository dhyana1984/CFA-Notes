# Central Limit Theorem 中心极限定理
中心极限定理就是对$\overline{X}$的概率分布进行了描述：  
对于任意均值为$\mu$，方差为$\sigma^2$的总体，假设简单随机抽样计算出样本均值为$\overline{X}$，样本容量为$n$，当$n\geq30$时，$\overline{X}$服从均值为$\mu$，方差为$\frac{\sigma^2}{n}$的正态分布  
**中心极限定理的三个条件:**
* 抽样必须是简单地随机抽样
* 总体的均值与方差均有限，不为无穷大
* 样本容量超过30  

**中心极限定理的三个结论**
* 样本统计量$\overline{X}$服从正态分布
* 样本统计量$\overline{X}$均值为$\mu$
* 样本统计量$\overline{X}$的方差为$\frac{\sigma^2}{n}$  

***注意，这里的$\overline{X}$的方差是$\frac{\sigma^2}{n}$而不是$\sigma^2$，因为$\overline{X}$的方差肯定低于总体X的方差$\sigma^2$，由于是n个数求平均，所以对应其系数$1/n$***  
# Confidence Interval Estimate 置信区间估计
区间估计是指估计未知总体参数的取值范围。给定概率水平$(1-\alpha)$，估计的confidence interval置信区间将以$(1-\alpha)$的概率覆盖未知总体参数，其中，$\alpha$称为significance level显著水平，$(1-\alpha)$称为degree of confidence置信度  
置信区间的宽度与置信度正相关，与显著性水平负相关  
## 置信区间的公式
$$
点估计量 \pm Reliability factor(置信因子)\times标准误
$$
* 当$\sigma^2$ 已知时，计算$\mu$的置信区间，假设总体服从正态分布，公式变为：
$$
\overline{X}\pm z_\frac{a}{2} \frac{\sigma}{\sqrt{n}}，z_\frac{a}{2}表示标准正态分布下\alpha/2的分位数
$$
**正态分布的几个置信因子：**  
90%置信区间，$z_\frac{a}{2}=1.65$  
95%置信区间，$z_\frac{a}{2}=1.96$  
99%置信区间，$z_\frac{a}{2}=2.58$   

* 当 $\sigma^2$未知时，计算算$\mu$的置信区间，假设总体服从正态分布，公式变为  
$$
\overline{X}\pm t_\frac{a}{2} \frac{s}{\sqrt{n}}，t_\frac{a}{2}表示自由度为n-1的t分布下\alpha/2的分位数
$$

***注意几点***  
1. 根据总体方差是否已知，判断用正态分布还是t分布构造置信区间
2. 氛围是是$\alpha/2$而不是$\alpha$
3. 标准误是$\frac{\sigma}{\sqrt{n}}$或者$\frac{s}{\sqrt{n}}$,而不是$\sigma$或者$s$
4. t分布的自由度变大时，概率密度函数会趋近于标准正态分布，只要n>=30，就可以利用标准正态分布分位数带入置信区间近似计算  

  
