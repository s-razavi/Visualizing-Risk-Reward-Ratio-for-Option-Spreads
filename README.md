# Visualizing Risk Reward Ratio for OptionSpreads

This code uses simple math calculations to visualize reward/risk ratio and facilitates finding the right strikes for long/short vertical option spreads:
Option contracts are exposed to time decay (extrinsic value of the option contracts). Time could be in favour or against the trade depending on the strikes of short/long spreads. The further a trader is bearish/bullish on a trade, the more he/she will agree to pay for the extrinsic value. 

Running the code requires few steps:

1- Obtain the option chain and corresponding spot price from your broker.

2- Define the extrinsic dollar value for the spread that suits your trading strategy:
  Negative: time decay favours you. 
  0: spread is not sensitive to time.  
  Positive: time goes against you if market does not move in your direction.

3- Run the code: it plots a heatmap showing values for the maximum_gain/maximum_loss ratios for any spread that satisfies the extrinsic value you agreed to pay.

Disclaimer: This code does not predict the market direction, neither it should be used other than educational purposes.
