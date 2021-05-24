# Mean 均值
## Arithmetic Mean 算数平均值，不适用于衡量多期(multi-period)的资产平均收益率
$$\mu = \frac{\sum_{i=1}^{N} {X_i}}{N}, \mu=总体均值，N=总体个数$$
$$\overline{X} = \frac{\sum_{i=1}^{n} {X_i}}{n}, \overline{X} = 样本统计，n=样本容量个数$$

## Geometric Mean 几何平均值
$$G = \sqrt[n]{X_{1}{\cdot}X_{2}{\cdot}X_{3}{\ldots}X_{n} } $$
当计算多期(periodic)平均收益率时，公式应该修改如下
$$Periodic{\;}return_{compound} = \sqrt[n]{(1+R_1)\cdot(1+R_2)\ldots(1+R_n)} -1$$

## Harmonic Mean 调和平均数，主要被用于计算定投的平均成本(cost averaging)
$$\overline{X} = \frac{n}{\sum_{i=1}^{n}{\frac{1}{X_i}}}$$

当$X_1=X_2{\ldots}X_n$时，$Harmonic\;Mean\;{\leq}\;Geometric Mean\;{\leq}\;Arithmetic Mean$    
&nbsp; 
# Dispersion 离散程度
## Absolute Dispersion 绝对离散程度
分位数是指位于数据中指定位置的数据，quartiles四分位，quintiles五分位，decile十分位, percentile百分位
$$ L_y = (n+1)\frac{y}{100}，n=数据个数，y=百分位点, L_y=分位数的位置$$ 

## Variance 方差
总体方差指数据与总体均值间距离平方的算数平均值
### 总体方差
$$\sigma^2 = \frac{\sum_{i=1}^{N}{(X_i-\mu)^2}}{N}$$
### 样本方差, 注意分母是n-1
$$s^2 = \frac{\sum_{i=1}^{N}{(X_i-\overline{X})^2}}{n-1}$$

## Standard Deviation 标准差
总体方差与样本方差开平方根以后得到总体标准差和样本标准差
### 总体标准差
$$\sigma = \sqrt{\frac{\sum_{i=1}^{N}{(X_i-\mu)^2}}{N}}$$
### 样本标准差
$$s = \sqrt{\frac{\sum_{i=1}^{N}{(X_i-\overline{X})^2}}{n-1}}$$
方差与标准差均反映了数据的离散程度，区别体现在量纲上

## Coefficient of Variation, CV 变异系数
变异系数剔除了量纲以及取值大小的影响。要就对象是资产收益率的话，变异系数表示单位均值收益率所承受的风险(单位收益下的风险)，因此在比对不同资产时，对于风险厌恶的投资者而言，变异系数越低越好
$$CV=\frac{s}{\overline{X}}，s=标准差，\overline{X} = 均值$$
## Sharp Ratio 夏普比率
夏普比率是衡量单位风险下的超额收益，对于风险厌恶的投资者来说，夏普比率越大越好
$$Sharp\;ratio = \frac{R_P-R_F}{\sigma_P}，R_P=资产P的收益率，\sigma_P=资产P收益率的标准差，R_F=无风险收益率，R_P-R_F=Excess Return\;资产P超过无风险收益率的超额收益$$

## Chebyshev's Inequality 切比雪夫不等式
切比雪夫不等式以标准差为衡量单位，给出了任意数据集离散程度的上界，对于任意一个方差$< +\infin$的数据集来说，其数据在均值k个标准差范围内的占比至少为$1-\frac{1}{k^2}$，其中$k>1$

# Skewness and Kurtosis 偏度与峰度
## Skewness 反应数据的对称性
$$样本的偏度是有关\sum_{i=1}^{n}(X_i-\overline{X})^3的表达式，反应数据的对称性$$
左偏时，均值<中位数<众数，右偏时，众数<中位数<均值
## Kurtosis 进一步衡量尾部的厚度
$$样本的峰度是有关\sum_{i=1}^{n}(X_i-\overline{X})^4的表达式，反应尾部厚度$$
* 峰度值高说明$X_i$偏离$\overline{X}$的极端值较多，尾部较厚，反之峰度值高说明$X_i$偏离$\overline{X}$的极端值较少，尾部较薄
* 正态分布的峰度为3，若峰度高于3，称为Leptokurtic 尖峰态，图形上比正太出现more peak and fat tail 尖峰肥尾巴
* 峰度低于3，则呈现为Platykurtic 平峰态，图形呈现出less peak and thin tail 矮峰瘦尾
* Excess kurtosis 超峰度 = 峰度 -3， 正态分布的超峰度 = 0,称为mesokurtic 平峰态，尖峰态的超峰度 > 0
$$
\begin{array}{|c|c|c|c|}
    \hline
    &\text{Leptokurtic} & \text{Mesokurtic}& \text{Platykurtic}\\
    \hline
    样本峰度&>3&=3&<3\\
    \hline
    超峰度&>0&=0&<0\\
    \hline
\end{array}
$$


