# Price slippage

### Author

[@paulapivat](https://twitter.com/paulapivat) (paul\_apivat#3817)&#x20;

### Description

The general definition of **slippage** is the difference between the expected price of a trade and the price at which the trade is executed \[1]. In a traditional order-book market, the term price impact describes what happens when the available liquidity of a prior limit-sell order impacts a subsequent limit-sell order at a higher price, resulting in the executed price being between the two limit-sell prices to which the order was filled \[2].&#x20;

There is a gap between expected price (i.e., price at limit-sell order time 1) vs. executed price (i.e., price between limit-sell order time 1 and time 2).&#x20;

The **price impact** in an AMM (automated market maker) context has a slightly different dynamic. While a trade is executed, the relative value of one asset in terms of another continuously shifts to where the final execution price is between where the price started and ended \[2].&#x20;

Moreover, the price impact for a given swap size will also change relative to the amount of liquidity available. Greater liquidity results in lower price impact, for a given swap size.&#x20;

Transactions submitted to Ethereum offering higher ‘gas’ fees are executed faster. Transactions with lower gas fees take a longer time. During this lag time, the relative value and available liquidity of the assets being traded could change, as other swaps take place.&#x20;

**Slippage tolerance** is the acceptable margin of change between price at time the transaction was submitted and pending, to the time the transaction was finally executed.&#x20;

Price slippage is, conceptually, a combination of price impact and slippage. And involves a combination of relative price, liquidity and gas fees.&#x20;

### References

1. Hayes, Adam (May 10, 2021). Slippage: What It Means in Finance, With Examples. URL: [https://www.investopedia.com/terms/s/slippage.asp](https://www.investopedia.com/terms/s/slippage.asp)
2. Uniswap V3 documentation: [https://docs.uniswap.org/protocol/concepts/V3-overview/swaps](https://docs.uniswap.org/protocol/concepts/V3-overview/swaps)
