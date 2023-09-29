# price_of_a_car

##### Problem: 
Car dealers want to know what feature in a car drives the price of a used car. To solve this by creating a model that should provide the best car features that predict the price of a used car. In order to solve this we need data on used car prices with all of its features.

The goal of the data mining is to gather the used car's various features and prices, and then process data to identify the patterns, then create a model to predict the important features.

The risk involved in this is the quality of the data, if the data has more noise then it needs to be cleaned until the data is good for modeling.

The steps that follow are:
* Understanding the data, and its noise.
* Cleaned the data and eliminated the unnecessary columns and rows, to reduce the complexity of the model.
* Prepare the data for modeling by further processing and tuning.
  
##### Modeling and Evaluation
The first model performed is sequential feature selection with linear regression, it resulted in a high MSE, such as

Train MSE: 154883939279135.88 and Test MSE: 181973336366337.2

And the model-predicted features are not that accurate.

After evaluating the first model, different techniques to perform the model to get better accuracy.

The second model performed is Redge with polynomial degree 2 transformation, which resulted in a slightly better MSE.

Train MSE: 154872421163766.16 and Test MSE: 181970357144187.6

The order of features most to least important predicated by the model are Manufacturer, Odometer, Type, Transmission, Drive, Cylinder, Condition, Pain_color, title_status, year, fuel, and size.

The feature selected by this model is more reasonable than the first model, and this can be brought back to the client.

##### Deployment
The top five features of a used car that drives the price predicted by the model are vehicle manufacturer, Odometer for miles vehicle driven, type, transmission, and Drive. Auto dealers can apply this as one metric to sell or by a used car. This can be monitored through future sales and optimized if necessary.
