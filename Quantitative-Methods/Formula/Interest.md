# Time Value of Money(货币的时间价值)
## Interest(利率)
* Interest Rate(利率) = Real Risk-Free Interest Rate(实际无风险利率) + Expected Inflation Premium(预期通货膨胀溢价) + Default Risk Premium(违约风险溢价) + Liquidity Premium(流动风险溢价) + Maturity Premium(期限风险溢价)  
* Nominal Interest Rate(名义利率) = Real interest Rate(实际利率) + Expected Inflation Premium(预期通货膨胀溢价)
* Effective Annual Rate(EAR,有效年利率), $r_s$ = Quoted Interest Rate(报价利率), m = interest in 1 year(1年内计息次数)，  $\frac{r_s}{m}$ = periodic interest rate(计息期利率)
$$ EAR = (1+\frac{r_s}{m})^m -1$$
## Present Value and Future Value(现值和终值)  
* r is Interest Rate, n is Interest Period(计息周期数)
* $FV=PV\times(1+r)^n$
* $PV=\frac{FV}{(1+r)^n}$
* **Ordinary Annuity(普通年金)**, 每期期末支付等额年金，例如，持续3年，利率为10%,每期支付200年金  
$$FV=200\times1.1^2 + 200\times1.1+200=662$$
$$PV=\frac{200}{1.1}+\frac{200}{1.1^2}+\frac{200}{1.1^3}=497.37$$
* **Annuity Due(先付年金)**，每期期初支付年金，例如，持续3年，利率为10%,每期支付200年金  
$$FV=200\times1.1+200\times1.1^2 + 200\times1.1^3 =728.2$$
$$PV=200 + \frac{200}{1.1}+\frac{200}{1.1^2}=547.11$$  
* **Perpetuity Annuity(永续年金)**, 无限期支付年金，支付年金的时间点是每期期末, A是每期期末支付年金金额，r是利率
$$PV=\frac{A}{r}$$

