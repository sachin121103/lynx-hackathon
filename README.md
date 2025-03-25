# Lynx-Hackathon

The objective of this Hackathon is to develop a simple trading algorithm
that operates within small time windows. Our algorithm should be designed
to maximize efficiency while considering market dynamics and competition
from other teams

## Key Concepts and Vocabulary

### Single Exchange Trading

All trading activity occurs on a single exchange, meaning that all buyers
and sellers interact within the same market. This is crucial, as our bot’s
decisions may be influenced by the strategies of other teams.

### Short-Selling

Short selling refers to holding a position with negative exposure. This means
that an asset is sold with the expectation that its price will decrease, allowing
it to be bought back at a lower price for a profit. When calculating returns,
the equations take into account the absolute value of the position X<sub>i,j</sub>

### Asset Volatility

Volatility refers to the extent of price fluctuations of an asset around its
average value. It provides insight into how drastically an asset’s value can
change. A related statistical measure is kurtosis, which captures the likeli-
hood of sudden, extreme price changes.

## Overview of the Algorithm

When designing the trading algorithm, three main components must be
considered: 

### Risk Management

To manage risk, we will use the adjusted Sharpe ratio. This metric
provides a percentage-based assessment of the risk associated with an in-
vestment. In simple terms, it evaluates the steepness of the return curve
and accounts for kurtosis (which measures the likelihood of sudden price
swings).

### Function Prediction

The algorithm must predict future asset behavior based only on available
historical data up to the current moment. Important: There is a risk of
data leakage—using future data improperly—which is strictly prohibited
and would lead to disqualification. To prevent this, we will run a validation
test that compares our predictions against actual market behavior.

### Decision Making

The bot’s decisions should be based on:

* Risk assessment using the adjusted Sharpe ratio.
* Predictions derived from historical data
* Market conditions, including interactions with other competitors.

These considerations will guide the bot in executing trades efficiently while
minimizing risks.

## Our Algorithm

TODO


