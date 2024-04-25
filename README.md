<h1 align="center"> Constructing Cointegrated Cryptocurrency Portfolios for Statistical Arbitrage </h1>

<head>

</head>
<body>
	<div class="banner">
		<img src= https://img.freepik.com/premium-vector/crypto-currency-horizontal-banner-bitcoin-digital-web-money-technology_48369-13318.jpg?w=2000 alt="ICO Types Banner">
	</div>
</body>

This repository contains the code and outputs of a python project carried out to create a cointegrated portfolio using four cryptocurrencies, with the aim of potentially reaping profits from an arbitrage opportunity.


The project was carried out based on the research paper titled "Constructing Cointegrated Cryptocurrency Portfolios for Statistical Arbitrage" by Tim Leung and Hung Nguyen. The paper proposed a methodology for constructing cointegrated portfolios of cryptocurrencies using a series of statistical tests, including the Johansen cointegration test and Engle-Granger two-step approach. The authors constructed cointegrated portfolios involving four cryptocurrencies: Bitcoin (BTC), Ethereum (ETH), Bitcoin Cash (BCH), and Litecoin (LTC) and developed several trading strategies under different entry/exit thresholds and risk constraints. The methodology can be applied more generally to create new cointegrated portfolios using other cryptocurrencies.

Please go through the article "Constructing Cointegrated Cryptocurrency Portfolios for Statistical Arbitrage" First

The four cryptocurrencies selected for the portfolio are Solana (SOL), Cardano (ADA), Ripple (XRP), and Binance Coin (BNB), with hourly data from 2021 acquired from Binance.com. A linear regression is run over the closing price data for the four cryptocurrencies, and the resulting regression equation is used to create a spread equation for trading and calculating profit/loss.

To ensure the stationarity of the residual terms, the augmented Dickey-Fuller (ADF) test, the Phillips–Peron (PP) test, and the Kwiatkowski–Phillips–Schmidt–Shin (KPSS) test are performed. After one round of differencing, all the four coins’ closing prices indicate stationarity.

The prediction for the values of coin prices is made using the Autoregressive Integrated Moving Average (ARIMA) model, and the parameters used for the model are defined.

The trading strategy used for calculating the arbitrage profit involves short-selling when the Spread at a time t is below the lower specified limit, and using the long position for the Spread increasing beyond the limit. Different values above and below the mean were tested, and it was found that a “c*σ” value of 0.75σ gave the highest profit margin i.e. 100k USD on an initial investment of 100,000 USD, giving an ROI of 100% over the given period.

The repository includes graphs and visualizations of the data, code for the analysis, and instructions for running the project. The results and conclusions drawn from the analysis are also included in the report.
