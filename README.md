🧭 **Project Overview**

In this project, I try to test what are the best investment strategies that a new passive investor should chose to allocate his money in. I try to estimate four strategies: Buy and hold; Day trading; Overnight trading; Buy and hold excluding the top 3 and worst 3 trading days in each year. We use the SPY ETF as our market proxy. We assume the investor is from Texas and is deciding on how best to allocate $10,000 starting January 1, 2024. The investor is looking to maximize returns while taking into account tax implications and market timing considerations. I backtest the strategies over historical data (from the first trading day of SPY in 1993) to compare their performance in terms of returns, volatility, and tax-adjusted profitability.

🎯 **Objective**

To identify the best-performing investment strategy among four SPY-based approaches by:
1. Backtesting each strategy's performance
2. Accounting for short-term capital gains tax and tax-loss harvesting
3. Evaluating risk-adjusted returns

🧠 **Assumptions**
1. The investor is based in Texas (no state income tax). 
2. A zero-commission brokerage is used. I assume no other transaction costs apply.
3. Taxes are applied only at year-end for short-term capital gains. 
4. Tax-loss harvesting is performed automatically and efficiently.
5. The $3,000 limit on tax-loss harvesting does not apply. 


💡 **Strategies Evaluated**
1. Buy and Hold: The investor holds and sells it at the end of the duration.
2. Day trading: The investor buys and exits after every trading day, and re-enters the next trading day with only the remaining money.
3. Overnight trading: The investor buys and exits after every overnight trading sessuib, and re-enters the next session with only the remaining money.
4. Buy and Hold with foresight: The investor buys and holds, and has the foresight in the experiment to know the best and the worst three days each year.

🔧 **Tools Used**
Python,yfinance, pandas, numpy, matplotlib, seaborn

📊 **Results**

Strategy 1:
This strategy suits a passive investor wanting to invest and forget about it for a long period of time. We conclude that even though the investor faced losses while extreme volatility like pandemic or 2008 financial crisis, the overall returns outweighs the associated risks. Overall profit after tax: 1740.86%

![image](https://github.com/user-attachments/assets/2eb1c5b0-db71-4ee0-b9d8-bcde735f6c97)

  
 _Pros:_
Low transaction cost ; Time saved ; Low taxes
  
_Cons:_
High opportunity cost ; Different strategy could be much more lucrative ; Chance investor can lose entire investment if there are no exits during recessions

Strategy 2:
This strategy is not won’t be fruitful for any type of passive investor either risk averse or a risk seeker. A risk averse person wouldn’t invest everyday if he/she knows a financial crisis is going on and at the same time, a risk seeker won’t be interested as well as he/she wouldn’t be getting the returns for the risk involved. There are more negative aspects like the transaction cost of trading as it would be absurdly high along with opportunity cost of missing the overnight market. Overall profit after tax: -1.90%. Only active investors should chose this strategy.

![image](https://github.com/user-attachments/assets/7756b622-5fc5-4b9c-bb45-7f42a1e18873)

_Pros:_ No overnight exposure; High liquidity ; Low opportunity cost - ability to pursue better opportunities if they arrise
  
_Cons:_ Emotional stress; Limited time horizon ; High transaction cost ; Market volatility

Strategy 3:
We believe that strategy 3 is similar in terms of strategy 2, no type of investor would go for a strategy like this since it is yielding negative profits at the end of 30 years. This strategy will not only decrease the liquidity but also incur a lot of transaction costs. Overall profit after tax: - 0.55%

_Pros:_ Early reaction to news; Opportunity for after hours gain; Potential for lower price volatility

 _Cons:_ Increased risk and volatility; Higher transaction cost; Missing out on lucrative intraday opportunities; Lack of liquidity

![image](https://github.com/user-attachments/assets/f06a0a58-0d65-4720-87f4-7f06029886c6)

Strategy 4: This strategy gave the best pre and post tax return on the market mainly due to removing the worst days like the dot com bubble crash, the 2008 crash, and the pandemic shocks. However, the tax compliance for this strategy would be very complex and the after-tax profits that we calculated(on the basis of short-term capital gains) are likely to be inflated. One of the main negative aspect of this strategy is the super-natural ability a person must posses to know the best and worst days is not possible in real life. Overall profit after tax: 1797.68%. This shows that a lot of the market returns are driven by outliers but these are impossible to predict.

_Pros:_ Exponential growth; Potential lower fee

_Cons:_ Foresight ability (impossible); High opportunity cost

![image](https://github.com/user-attachments/assets/12f8f1c5-cb82-404c-b05d-618d1a636e63)

**Risk Free Alternative?**

What if there was an alternative to invest in a risk-free asset like a 30-year T-Bond. 
Assuming the treasury bond in issue at the same time as the first SPY ETF is Zero Coupon, the YTM would 7.2%. The investor also doesn’t really have an opportunity to profit of potential price fluctuations as the YTM is flat compared to the exponential growth witnessed by the SPY ETF. Even if we relax the assumption of no coupons, generally the coupon rate tracks the YTM closely. Therefore, holding only T-bonds would not yield the investor sufficient returns.

![image](https://github.com/user-attachments/assets/73f6eb5b-e3de-4c3b-9b36-6c97d87a986e)


📌 **Conclusion**

After careful assessment of all the four strategies presented to us, our favor would go in the direction of strategy one or strategy four purely on the basis of the profits. But there are few reasons why to believe that strategy 1 would still be better than strategy 4, such as: 
The assumptions used for calculating tax in strategy four is extremely simple for the complex nature of STCG, relaxing the assumptions like the no yearly harvesting limit itself will reduce the profits.
Biggest shortcoming of strategy 4 is its foresight ability which is not possible in a real-life scenario. 

![image](https://github.com/user-attachments/assets/69850452-b402-4a9f-af4b-74f02ca15851)



