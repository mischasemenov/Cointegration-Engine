# Vectorized Cointegration & Statistical Arbitrage Engine

**Date:** 11 August 2026

---

## 📌 Overview
This project investigates a co-integrated pair of stocks with a goal to create a trading strategy based on the linear relationship. The final pair consists of Class A voting shares (GOOGL) and non-voting Class C shares (GOOG), which creates a dual-class co-integrated pair which we can profit from. We then calculate the average mean-reversion and the look-back window via the discrete Ornstein-Uhlenbeck Process. The strategy consists of going long when the Z-score is below -1.25 because that means that the Class A shares are underpriced relative to its non-voting counterpart, and short otherwise.

---

## Results: 
We assume 0.0001$ of transaction costs per trade. Our results show a modest decay of the Sharpe Ratio from 2.19 to 2.14 when we apply the algorithms OOS. Importantly, our annualised volatility has dipped slightly to 1.62% from 1.84%. Consequently, our Sharpe Ratio has retained 97.7% of its in-sample efficiency. With a tightly contained loss of ~1$ which means that strategy is successful. To showcase this, I have prepared two graphs represent the dual equity curve plot and the maximum drawdown chart.

              Sample  Trading Days Total PnL  CAGR Ann. Vol Max Drawdown Sharpe Ratio Calmar Ratio
   In-Sample (Train)           450     7.43% 4.10%    1.84%       -0.96%         2.19         4.20
Out-of-Sample (Test)           804    11.63% 3.51%    1.62%       -0.96%         2.14         3.62
         Full Sample          1254    19.93% 3.72%    1.70%       -0.96%         2.15         3.82

## Equity Curve starting at 1$
![image alt](https://github.com/mischasemenov/Cointegration-Engine/blob/f2ca88e3ef4573e7cb36312f5d2d4854d23283d7/output.png)

## Maximum Drawdown Profile
![image alt](https://github.com/mischasemenov/Cointegration-Engine/blob/19dfc4cabe1d961e7027581ae1acddc91248f312/maximum_drawdown.png)
---

## 📬 Contact

If you have questions or suggestions regarding the methodology or execution, feel free to reach out (no spam please):

* **Author:** [Mikhail Semenov]
* **Email:** [ms624@st-andrews.ac.uk]
