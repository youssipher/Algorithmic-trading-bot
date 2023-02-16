# Trading-strategy
We present a trading strategy, combining several approaches, and apply it on Brent price.
The general framework we will follow is about predicting an unknown sequence, using a combination of experts, more or less trustworthy. 
During the process, the goal of the operator is to determine which experts are reliable, in order to use their predictions.
Here, in order to be more robust and simulate the use of various information sources (price of correlated stocks, macro event in the market etc...) our experts will be different trading strategies. The level of trust of each of them will be represented by a weight (real number). If an expert performs well (we explain in the notebook what 'perform well' means), his weight increases and vice-versa.
A global reference of prediction using experts advices can be found in "Cesa-Bianchi, N., & Lugosi, G. (2006). Prediction, learning, and games. Cambridge university press".
