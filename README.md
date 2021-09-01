# Retirement Financial Planning
Background Storyline: You decided to start a FinTech consultancy firm, and you want to make a difference by working on projects with high social impact in local communities. You just won your first contract to help one of the biggest credit unions in your area. They want to create a tool that helps their members enhance their financial health. The Chief Technology Officer (CTO) of the credit union asked you to develop a prototype application to demo in the next credit union assembly.

The credit union board wants to allow the union's members to assess their monthly personal finances, and also be able to forecast a reasonably good retirement plan based on cryptocurrencies, stocks, and bonds.

For this storyline, I have focused on using APIs as part of the technical solution - to create two financial analysis tools.

The first will be a personal finance planner that will allow users to visualize their savings composed by investments in shares and cryptocurrencies to assess if they have enough money as an emergency fund.

The second tool will be a retirement planning tool that will use the Alpaca API to fetch historical closing prices for a retirement portfolio composed of stocks and bonds, then run Monte Carlo simulations to project the portfolio performance at 30 years. I have then use the Monte Carlo data to calculate the expected portfolio returns given a specific initial investment amount.


## Project Details

Please note that Simulations can be re-ran for different dates and portfolio weightage to generate alternate Results.

### 1) [Part 1 - Personal Finance Planner](financial-planner.ipynb)
### Results:
> Combined Portfolio of Crypto Assets (Bitcoin and ETH), and Traditional Stocks (SPY) and Bonds (AGG) compares well against the Emergency Fund target of 3 times the Monthly Income of USD 12000

### 2) [Part 2 - Retirement Planning](financial-planner.ipynb)
### Results:


> For a 40/60 portfolio of Bonds (AGG) and Stocks (SPY):
>> There is a 95% chance that an initial investment of USD 20000.0 in the portfolio over the next 30 years will end within in the range of USD 572510.84 and USD 3226709.24.
>>
>> There is a 95% chance that an initial investment of USD 30000.0 in the portfolio over the next 30 years will end within in the range of USD 858766.25 and USD 4840063.86.


### 3) [Early Retirement](financial-planner.ipynb)

### Results:

> Upon adjusting the portfolio to either include more risk (a higher stock than bond ratio) or to have a larger initial investment and rerun the retirement analysis to see what it would take to retire in 5 or 10 years instead of 30!

> For a 05/95 portfolio of Bonds (AGG) and Stocks (SPY):
>> There is a 95% chance that an initial investment of USD 520000 in the portfolio over the next 5 years will end within in the range of USD 1052691.14 and USD 3143232.08.

> AND

> For a 20/80 portfolio of Bonds (AGG) and Stocks (SPY):
>> There is a 95% chance that an initial investment of USD 220000 in the portfolio over the next 10 years will end within in the range of USD 819595.32 and USD 3258919.6.

References:
[Monte Carlo Simulation Library file](MCForecastTools.py/)

