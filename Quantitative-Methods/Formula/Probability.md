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
