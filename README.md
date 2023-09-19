# # Data Projects

#Pinescript Strategy:

Changed variable contents for strategy privacy. Produced current winrate of 68%, max drawdown of 67%, profit of 750%, and Sharpe ratio of 0.31. 

Strategy analyzes a pattern of cosecutive candles with a particular pattern of increasing candle sizes among previous x number of candles. A hard exit of x number of points is placed above and below the purchase price, minimizing drawdowns. Selling contracts is not permitted with this strategy as I found it decreases winnings. 

Strategy produces consistent winnings, but to further minimize any drawdowns, it needs to be a lot more consistent with the right measurement of the exit sizes that adapt to current bars. This is difficult to calculate in live markets as different hours and different days can produce completely inconsistent patterns making it difficult to predict the right sizes for exits. Looking to incorporate a machine learning model that can input data from previous days and months to calculate a required candle size for each time period while cleaning data for large inconsistencies that should be ignored. 
