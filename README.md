# Stock-Market-Volume-Analysis

In this repository we attempt to determine the possible relation between volume and price on S&P 500. In attempting to establish this relationship, we asked ourselves the following:

- on days with greater volume would there be a larger range between the high and the low of the day?

- on days with greater volume would there be a larger range between the opening and closing price for the day?

First we ran our linear regression model on the entire S&P 500 over a 7 year period, but we ran into the problem of split-adjusted stocks where there would be an extreme change in price without a corresponding change in volume. This massively skewed our model, so we decided to run the model again, this time on Apple's stock, within an isolated time period where there wasn't the issue of split-adjusted data. This significantly improved our model. Two interesting results were:

- the difference between the high and low of the day increased the greater the volume.
- the difference betwee the open and close of the day decreased on days with greater volume. 

These are some very curious results which might indicate more extreme volatility on days with higher volume where heavy buying and heavy selling might both occur on the same stock on the same day. 

Future iterations of this analysis will include using split adjusted data and creating a field for for a 20 day moving average of relative volume. 
