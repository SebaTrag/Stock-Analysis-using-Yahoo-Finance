# Stock Analysis using Yahoo! Finance

<b>Group Project <br>
3,793 | 4,799: Skills<br>
Programming - Introduction Level <br>
Autumn Semester 2019 <br>
Dr. Mario Silic <br>
University of St.Gallen </b> <br>
<br>

##	Project Overview

### Goal of our programming project
The goal of this project is to provide the user a tool to visualize stock data of selected companies based on the Yahoo! Finance database and therefore analyze stocks to form an individual portfolio. 

### Motivation for working with Yahoo! Finance
Most of our group are really interested in finance and have heard from many sources that programming will become more and more important in the future. Since one part of the course was to code an own project, we wanted to combine our interest in finance with our new programming skill set and therefore decided to work with Yahoo! Finance. 

### Project Deliverable
The project deliverable is the file <i>Stock Analysis using Yahoo! Finance.ipynb</i> - the source code for the Python program. Therefore, the user must install “Jupyter Notebook” first. For further information please visit the website: https://jupyter.org/.
<br>
<br>
<br>

## Basics of our program

To start off the program, one must install all the libraries, followed by restarting the kernel, before importing the libraries and creating the color class. The user then can input the stock symbol and can choose from up to seven options to perform the analysis:
- Display the price chart of the stock
- Get a price comparison with an additional stock
- Get the earnings and revenue statement of the chosen stock
- Get the cash flow statement of the chosen stock
- Receive the analyst recommendations for the stock of the last six months
- Get the price prediction for the next 30 days (based on historical data) <br>

Also, the user can quit the program anytime by selecting option ‘Q’: Quit the program. Below is the description of each option used for stock price analytics:

<ul type="square">
<li><b>Option A</b>: <i>"Show me the price chart of the stock"</i><br>Plots the time series of selected stock prices in an interactive graph.</li>
<li><b>Option B</b>: <i>"Show me a price comparison with an additional stock"</i><br>For comparison, plots the time series of the selected company stocks on a single interactive graph.</li>
<li><b>Option C</b>: <i>"Show me the earnings and revenue statement of my chosen stock"</i><br>Shows the earnings and revenue statement of the chosen stock for the last 4 years plotted into a bar chart.</li>
<li><b>Option D</b>: <i>"Show me the cash flow statement of my chosen stock"</i><br>Shows the cash flow statement of the chosen stock for the last 4 years plotted into a bar chart.</li>
<li><b>Option E</b>: <i>"Show me the analyst recommendations for the stock of the last 6 months"</i><br>Shows the percentage of analysts’ recommendations in categories “hold”, “sell”, “buy”, ”neutral”, “outperform”, “underperform”, “market perform“, overweight” and “underweight” in a pie chart.</li>
<li><b>Option F</b>: <i>"Show me the price prediction for the next 30 days"</i><br>The price prediction is based on the past values of the stock. The prediction is done fitting a linear regression model on the past data. Linear regression is a simple technique and quite easy to interpret, but there are a few obvious disadvantages. One problem in using regression algorithms is that the model overfits to the date and month column. Instead of taking into account the previous values from the point of prediction, the model will consider the value from the same date a month ago, or the same date/month a year ago.<br>For the forecast we used the instructions from the article <i>"Predict Stock Prices Using Python & Machine Learning"</i> (https://medium.com/@randerson112358/predict-stock-prices-using-python-machine-learning-53aa024da20a).</li>
</ul>

(<i>Note that the program provides a simple tool for stock price analytics since the project’s goal is building a Python program rather than a financial model. For better valuation and prediction of stock prices, the given models need to be adjusted and calibrated for all factors.</i>)<br>

We have also provided you with a list of the most popular stocks at the bottom of our code.
<br>
<br>
<br>

## Problems and Summary
In this section we want to elaborate on two main problems which occurred during our coding stage and how we got to solve them. Since we first wanted to implement a valuation model into our programming, like the discounted cash flow valuation or the residual earnings valuation, we found out that Yahoo! Finance does not provide any kind of forecasts for the free version. This was a huge problem for us since these two mentioned models rely on highly accurate forecasts. Therefore, we had to change our original plan with two different options, which is why we implemented the cash flow statement as well as the revenue & earnings statement, since they are crucial to form a fundamental analysis. The second problem was that some stocks within Yahoo! Finance were not saved within the same data frame structure, which gave us problems with importing data. We later found out, that this was only happening with around five to eight percent of the most popular stocks, which is why we decided to delete stocks which had a different data structure (e.g. AAPL, NKE & AMZN).<br>

In conclusion we really enjoyed the programming project and the course in general. The most fun part of the course definitely was the coding project since we were able to work with real data and actually write a program by ourselves. It gave us an insight in how to get from a raw data structure to a meaningful visualization and gave us the tools to maybe use programming more often for upcoming papers.
<br>
<br>
<br>

## Authors
<b>Gyozalyan Zhasmina</b><br>
<b>Rizzi Flavio</b><br>
<b>Scarascia Florian</b><br>
<b>Tragust Sebastian</b><br>
<b>Wirth Alain</b><br>





