# Options-pricing
In this notebook, we estimate option prices in the Black Scholes model. The data consists of option prices for call and put options for the S&P500 index and has been retrieved from Yahoo finance (https://finance.yahoo.com/quote/%5EGSPC?p=%5EGSPC) over several days in Januray 2020. 

The first step is to find the implied volatilities using Newton's method. After that, we split the datasets and perform a linear regression on each part. This gives us a piecewise linear approximation that takes volatility smiles into account. We compute the Black-Scholes price for this approximation and compare it to the observed option prices.  


