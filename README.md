# Stock portfolio and Property analyser

Team members: Shavan Patel, Kevin Chen, Arian Zehtab


## PROJECT DESCRIPTION
---

This program is a combination analyser for both a stock portfolio and property investment

### Stock Portfolio Analysis:

To analyse your stock portfolio we will take in a csv of your stock trading history with symbols, date of trades, order type (buy/sell), and volume traded.
We will also need the initial value of your investment.

We will return the valuation of your portfolio over time, as well as chart your returns, and a box spread of your returns. The program will also calculate the standard deviation, and annualized standard deviation, as well as the sharpe ratio of your portfolio. 

### Property

To find details regarding your property, enter in your address and the program will automatically find the closest match for what you typed in.

We will show the median sale price and approximate number of properties sold in your suburb


---
Help user get total ROI of all investments

Help the user see historical data for his investment

Help user compare investment performance and composition between investment types

Help user analyse individual investment performance specific to each type
---

---
Below is a summary of things we think we can do with the program
---

## STOCKS 
BASE
---
*merge data for analysis*

Input: history of all purchased  stocks, purchase date, broker fee, closing price

Analysis: ROI, investment history (line graph), portfolio composition (pie), sharpe ratio (against ASX200, or S&P500), + all stock analysis from hw,
    comparative stock performance

Potential analysis: Dividend calculation

## CRYPTO
*merge data for analysis*

Input: history of all purchased  stocks, purchase date, broker fee, closing price

Analysis: ROI, investment history (line graph), portfolio composition (pie), sharpe ratio (against USD), + all stock analysis from hw
    comparative stock performance

## FOREX
*merge data for analysis*

Input: history of all purchased  stocks, purchase date, broker fee, closing price

Analysis: ROI, investment history (line graph), portfolio composition (pie), sharpe ratio (????), + all stock analysis from hw

## PROPERTY

Input: purchase price, purchase address(COUNTRY (AU at minimum), STATE, CITY, COUNCIL, ???)(this depends on domain API restrictions),

Extension: loan amount, loan rate, loan premium

API data we hope we will get:

Analysis: purchase price compared to average price (both at time of purchase and current), total increase in price

Extended analysis: ROI adjusted for loan



### Overall

Overall analysis: portfolio composition (start and current)

## Datasets

Alpaca for stock and crypto

Domain for property

## Questions 

Questions for Users (Property)
1. How is my property performacing compare to the valuation?
2. What is the average price for similar houses?
3. Rent vs Average/median rent in the area?
4. Visual images and garph on how my propety is peformancing 
5. Cap Rate of the investment? or Gross Yield?
6. Opinion on wheather I show to sell the property or keep the property 
