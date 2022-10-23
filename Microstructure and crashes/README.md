
# VPIN orderflow toxicity
VPIN = Volume synchronized Probability of Informed trading

Used to predict the flash crash of 2010, 1 hour in advance. (E-MINI S&P 500)

PIN = Probablity of Informed trading

Wih sequential trading model with bayesian updates the authors proposed a  Market Microstrucure theory system that can explain the range at which MMs are willing to provide liquidity. This can be used to detected puking/toxic orderflow


# The Inelastic Market Hypothesis: A Microstructural Interpretation

Suppose that the only thing that can move prices is fundamental value, the price *should* stay constant until there is some new information, public or hidden that impacts the fundamental value and thus move price. However looking at a price chart at any given day for any given traded asset. Intraday and long term does seem to not agree with this, there is too much "noise" and trendyness for this to be true. 

```
It's just orderflow -> "More buyers than sellers" -> The price adjusted higher until supply met demand.
```

Besides, Market making would fundamentally be unprofitable if the market was always efficient and price only moved because fundamental valuation changed.

Markets are feedback-loop heavy <=> highly volatile in abscense of news

\>80% of market volatility is self-generated.

```
Buying(selling) 1$ worth of a stock changes the marketcap by M$ longer term, where M = 1;
Buying(selling) 1$ worth of an index changes the marketcap by M$ longer term, where M rougly equals 5;
```

## Undergraduate example

When an investor sells one dollar of bonds to invest in a representative asset mangager with a a mandate of keeping 80 % of its invetments in stocks, the price of stocks has to increase, in equilibrium, by five dollars, corresponding to 
$(1-80\%)^{-1} = 5$


## High Frequency Price Impact
Price impact: Takers hitting the resting orders, market buy order hitting the asks or market sell order hitting the bids.

There are two strands of though for price impact, the two extremes are:

1. **Agents successfully forecast short-term prcie movements, and trade accordinlgy.**
    
    This essentially just means efficient market theory, someone has information that that changes the underlyings valuation from the current valuation. Orders are then executed to reflect that difference. 

2. **Price impact is a reaction to oderflow imbalance** 

    Fundamentals are BS the literal only thing that matters is, where is supply and where is demand and price will be a function of that. Some dude likes the stock and apes -> more dudes who sees short term volatility gets ape brain neurons activation -> price gets bid -> price rapidly to new supply area where it equalizes. Does it matter that the stock had a shady CEO? Or that the projected earnings where bad? No.

This might seem like a self-fullfilling prophecy of sorts but the paper goes on to show that the information per trade is quite small.

## The Square-Root Law
When larger entities execute metaorders (micro-orders routed with volume Q over time T, through limits and or taking). The price impact is not lineary but closer to square-root
