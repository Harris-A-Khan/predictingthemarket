### Introduction

	Data fuels the modern world. Large corporations, from Facebook to Google, rely on the data of individuals to understand and target consumers and users in the cloud. The majority of data processing is done with computers, afterall, computers are exceptional at data analysis; they can analyze thousands of  pieces of data in an instant, draw conclusions, find patterns, extrapolate, and predict. The methods by which this is done has advanced over the decades— manual and repetitive input and analysis of data has been replaced by machine learning models capable of much more. 

	In this project, we wanted to explore the ways we could use a certain type of machine learning model to make predictions about a specific stock, in this case Microsoft. 

### Content
Initial Problem 
The Model 
Datasets
Results 
Conclusion
### Initial Problem

The question we wish to answer is very simple: can we predict day-to-day opening prices for Microsoft's stock. 

### The Model

There are countless machine learning models, each with its own pros and cons. We decided to go with a model known as Long Short-Term Memory (LSTM), a type of Recurrent Neural Network (RNN). Why this model? For several reasons.

The point of a stock analysis is to use trends in the data to predict future prices. A model that is incapable of taking into account past data (such as in the past 10, 15, or 30 days) is useless to us. Past data is key here. 
LSTM models give us a simple way to process entire sequences of data (also known as time series data) and lets us extrapolate the following day(s)
Vanilla RNN’s have a problem with a vanishing gradient, in other words the learning completely dissipates as the data reaches the end of the neural network. LSTM’s deal with this problem effectively by adding a unique additive gradient structure. 

### Moving Forward
	There are many different directions we could take this project in the future. We still aren’t very satisfied with the accuracy of our predictions. There are many ways we can go about tweaking the accuracy, though all involve trial and error:
	The first thing we thought about trying was using a different company’s stock. Under our current models, the predictions didn’t seem to pick up on patterns in the opening prices. The model performed very well when it came to predicting the training data, but when it came to predicting new data, it performed poorly. We think this happens because Microsoft stock is too volatile and unpredictable—there are no repeating patterns in the long-term. Perhaps a different company’s stock, specifically one outside the tech industry, would react differently to certain indicators and in turn become more predictable. Or, instead of just using one stock’s price, we use multiple and see if our model can pick up on trends between both sets of data.
	Regardless of which stock we choose to continue this project with, there are many changes we can make in creating our model.  


### Citations

In this project, we gathered data and code from a variety of sources. Our large set of opening data was taken from:

https://www.kaggle.com/borismarjanovic/price-volume-data-for-all-us-stocks-etfs

Our set of monthly unemployment rates was taken from:

https://www.kaggle.com/tunguz/us-monthly-unemployment-rate-1948-present

Our set of monthly housing starts was taken from:

https://fred.stlouisfed.org/series/HOUST

And lastly, many of the functions of our code was adapted from:

https://github.com/krishnaik06/Stock-MArket-Forecasting

