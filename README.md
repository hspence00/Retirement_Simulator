# Retirement Calculator
# Introduction

Our retirement calculator will allow a user to input their own financial data and determine if they will have enough funds to live comfortably throughout their retirement or allow them to make the adjustments to their spending based on their portfolio to ensure they do not run out of money in the future. 

Within the project the user will be prompted to provide information about the amount of money they currently have saved, they'll have multiple options of portfolio makeups to choose from along with the amount of years they anticpate being retired.  With that information our caclulator will run simulations with data being input from multiple historical data sources dating back to 1928 to determine if they'll have the funds to avoid running out of money in retirement.  

# Technologies

The following technologies are what is required to run our program:

- Python 2.7

# Historical Data

The data we used was pulled from the following sources listed below and input into our repository.  All data is annualized and begins in 1928 thus allowing the simulation to pull data that has mulitple financial cycles included.  This will ensure the simulation provides outputs that also have a variety of financial cycles thus providing an accurate representation of future posibitlies. 

We have broken down this information into the following catagories: Stocks, Bonds (10 Year T Bill rate), a 60/40 stock/bond ratio, a 50/50 stock bond ratio and a 40/50/10 stock bond cash ratio.  The user is prompted to select one of those options initially within our code. 

 - https://www.spglobal.com/spdji/en/indices/fixed-income/sp-us-treasury-bond-current-10-year-index/
- https://www.spglobal.com/spdji/en/indices/fixed-income/sp-us-treasury-bill-0-3-month-index/
- https://finance.yahoo.com/quote/%5EGSPC/history/
- https://www.nasdaq.com/market-activity/index/spx/historical
- https://home.treasury.gov/interest-rates-data-csv-archive
- https://www.investing.com/indices/us-spx-500-historical-data
- https://data.gov/
- www.macrotrends.net
- https://indexes.morningstar.com/page/resources
- https://pages.stern.nyu.edu/~adamodar/New_Home_Page/datafile/histretSP.html

# Monte Carlo Simulation

Monte Carlo simulation gives users an opportunity to view future possibilities based on histroic data.  Instead of just using one simulation it allows users to run thousands of simulations creating a greater overall picture of what could come. By tracking the amount of times the simulation predicts the input data is returned with a bankrupt reading out of 50,000 we can determine the probablity that the user will have sufficent savings to surving their expected retirement.  


# How To Use

Users  input will be python main.py to run our retirement calculator that is very user friendly. Runing the code the user will be prompted to input the initial value of their portfolio at the time of retirment, the amount of money they plan on withdrwaling annually and their minimum, expected and longest retirement periods (in years).  Our simulation will take that user inputted data, run it through the Monte Carlo simulation determine the likelihood of running out of money and print a chart for that individual scenarios calculation. 

Initial Investment = Starting amount of user funds.
Annual Withdrawal = Yearly spending of user.
Years in Retirement = Miniumum - Average - Max years in retirement for user.  In the user interface this item is simplified to a single average number. 
Investment Type = Which portfolio the user would like to run simulations on. 

# User Interface

Our teams graphical user interface acts as a widget to quickly and easily test out a plethora of combinations for your starting investment, your yearly spending, and the amount of years you plan to be retired for. It also allows you to select your investment type via a button click. This widget will allow the user to test out many different financial situations that they may be in and run a monte carlo simulation that goes through 5000 different lifetimes.  

# Future Enhancements

Our project could be imporoved by giving uses a greater variety of investment models to choose from such as cryptocurrencies, NFT's or gold or a user selected mixture of all of those options.  With more time the user interface would be updated to allow for additional customization within portfolios so that it would fit a greater number of users. 



