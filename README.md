# Retirement Calculator
# Introduction

Our retirement calculator will allow a user to input their own financial data and determine if they will have enough funds to live comfortably throughout their retirement or allow them to make the adjustments to their spending based on their portfolio to ensure they do not run out of money in the future. 

Within the project the user will be prompted to provide information about the amount of money they currently have saved, they'll have multiple options of portfolio makeups to choose from along with the amount of years they anticpate being retired.  With that information our caclulator will run simulations with data being input from multiple historical data sources dating back to 1928 to determine if they'll have the funds to avoid running out of money in retirement.  

# Technologies

The following technologies are what is required to run our program:

- Python 3

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

# Portfolio Analysis

Below you will see a financial analysis of the 5 portfolio types. The different visualizations used will help the user understand how the portfolios compare to eachother. In order to make a better judgment in which portfolio type the user wants to use. The 4 visualizations include Exponential Weighted Average (EWM), Cummulative Returns, Box and Bar graph to display Standard Deviation characteristics. Viewing these graphs identify key charactersitics about how these portfolios perfrom, and how they are different. 

Cummulative Returns

![Screen Shot 2022-09-11 at 5.05.17 PM.png](https://github.com/hspence00/FinTech_Project_1/blob/main/Images/Screen%20Shot%202022-09-11%20at%205.05.17%20PM.png)

Bar Graph (Standard Deviation)

![Screen Shot 2022-09-11 at 5.05.36 PM.png](https://github.com/hspence00/FinTech_Project_1/blob/main/Images/Screen%20Shot%202022-09-11%20at%205.05.36%20PM.png)

Box Plot (Standard Deviation)

![Screen Shot 2022-09-12 at 5.20.54 PM.png](https://github.com/hspence00/FinTech_Project_1/blob/main/Images/Screen%20Shot%202022-09-12%20at%205.20.54%20PM.png)

Exponentially Weighted Average

![Screen Shot 2022-09-12 at 5.21.23 PM.png](https://github.com/hspence00/FinTech_Project_1/blob/main/Images/Screen%20Shot%202022-09-12%20at%205.21.23%20PM.png)


# Monte Carlo Simulation

Monte Carlo Simulation gives you a more realistic assessment of how the future may unfold by looking at a wide variety of potential market scenarios that take fluctuating market returns into account. Instead of basing calculations on just one average rate of return, we generate thousands and thousands of simulations of hypothetical market scenarios, and calculate the impact on your savings during your retirement. Each simulation includes up and down markets of various lengths, intensities, and combinations 

When predicting outcomes 30 to 40 years into the future can be a challenge.  We are better off trying to keep things simple and focus on the most important and controllable issues. You can control when you retire, your investment asset allocation, how much you save, and how much you spend, but you can’t control the stock market, interest rates, and inflation.

# The pseudocode

![pseudocode](https://user-images.githubusercontent.com/109116465/189839414-90656585-0a51-4345-a840-db1b35eff207.png)

# How To Use CLI simulator

Users input will be python main.py to run our retirement calculator that is very user friendly. Running the code the user will be prompted to input the initial value of their portfolio at the time of retirment, the amount of money they plan on withdrwaling annually and their minimum, expected and longest retirement periods (in years).  Our simulation will take that user inputed data, run it through the Monte Carlo simulation determine the likelihood of running out of money and print a chart for that individual scenarios calculation. 

Investment Type = Which portfolio the user would like to run simulations on.

Initial Investment = Starting amount of user funds.

Annual Withdrawal = Yearly spending of user.

Years in Retirement = Min - Ave - Max years in retirement for user.

Input number of Monte Carlo Simulations (MCS) to run.

![Sim_image_2](https://user-images.githubusercontent.com/109116465/189823952-0ffef930-1257-4172-927c-ecdbcd258342.png)

![Sim_image_3](https://user-images.githubusercontent.com/109116465/189824549-375c69bf-6c61-49fe-8422-112ba643f7a7.png)

![Sim_image_4](https://user-images.githubusercontent.com/109116465/189825837-929ac781-6195-4b68-a4cc-4346092be534.png)


# GUI User Interface (BETA)

Our teams graphical user interface acts as a widget to quickly and easily test out a plethora of combinations for your starting investment, your yearly spending, and the amount of years you plan to be retired for. It also allows you to select your investment type via a button click. This widget will allow the user to test out many different financial situations that they may be in and run a monte carlo simulation that goes through 5000 different lifetimes.  

![GUI](https://user-images.githubusercontent.com/109116465/189824865-222a759b-5d3d-4f09-8e68-67ea8179da80.png)

# Future Enhancements

Our project could be improved by giving uses a greater variety of investment models to choose from such as crypto currencies, NFT's, gold or a user selected mixture of all of those options.  With more time the user interface would be updated to allow for additional customization within portfolios so that it would fit a greater number of users. 



