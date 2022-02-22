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

To find details regarding your property, enter in your address and the purchase price of your property, and the program will automatically find the closest match for what you typed in.

We will show the median sale price and approximate number of properties sold in your suburb, and compare this against your purchase price

## Instructions
---
Open main.ipynb and run all cells from top to bottom

At the bottom you will be presented with some tabs and text fields or a file upload button.

![Text Fields](Images\Text-Fields.png)

Property and Stock analysis is split up between the two tabs, you can switch between them using the tabs above.

Fill in all input prompts as instructed

## Restrictions on input
---
Although the input fields do not limit you on what you enter, there are a few limitations on what you can put in them for the program to function.

### Property

You can technically type anything into the text field, but the api call may not always be able to find the address you're looking for. The program will let you know what property it found with the address you entered. If no property is found at all it will also let you know.


The purchase price of your property must be a number. If the program does not receive a number it will let you know

### Stock Portfolio

The program will limit you to uploading csvs only, but your csv will need the following columns: [symbol,date,amount,order].

If one of these columns are missing the program may break

The program is designed to handle most cases where bad entries are made to the csv. If a symbol does not return data from the Alpaca Api it will be ignored.
If a given amount is not an nunber, or the order is not a buy or sell, it will ignore this particular entry.
If the date is not in a date format it may break the program


The Initial Value of your property must be a number. If the program does not receive a number it will let you know

## Some Notes on interpreting analysis
---
### Property

Make sure you check that your property has been found, your address and property type should be listed below. If the information is incorrect, the api may not have received enough information regarding your property, or it is not listed in the api database.

![Text Fields](Images\property-check.png)

The first two graphs show information regarding the sale number and sale price of property specific to your property type.

![median sold](Images\Median-Sold-Price-over-Time.png)
![property sold](Images\Property-Sold-over-Time.png)

The third graph compares your property purchase price with the median sold price of your property type over the last few years

### Stock

All data uses the total valuation of your portfolio.

![valuation](Images\Portfolio-Value-over-Time.png)

The first graph charts your portfolio's total valuation over time. This is calculated by adjusting your liquid valuation according to the buys and sells you made, and combining this with the total valuation of your stocks.

![change](Images\Portfolio-Change-Over-Time.png)

The second and third graphs are displays of the change in valuation of your portfolio. The first shows only change, the second shows the cumulative change over time

![cum returns](Images\Portfolio-Cumulative-Return.png)

For risk we display a box spread which shows your distribution of movement of the portfolio.

![box spread](Images\Box-Spread-of-Change.png)

Underneath is the standard deviation and annualized standard deviation, which is a numerical measure of how spread out the distribution of movement is on the portfolio

Underneath that is the sharpe ratio, which is a measure of how much return you are getting in comparison to your risk.