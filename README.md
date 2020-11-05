# House_prediction-Project
This project consists of two approaches to predict the price of a particular household in the US, first one is using the Linear Regression Machine-Learning model while another includes a deep-learning neural network model. We have taken two datasets for consideration so that we can compare the two models properly and able to perform descriptive and inferential analysis. 
One of the datasets contains house sale prices for King County, which includes Seattle. It incorporates homes sold between May 2014 and May 2015. It's an amazing dataset for evaluating simple regression models with over 20 features in total. For this particular dataset, a decent amount of exploratory data analysis and data pre-processing needs to be done, along with feature selection engineering. While for the second dataset with information about a bunch of houses in regions of the United States, this contains five features, so a little amount of exploratory data analysis and pre-processing would be suitable to work with this kind of data. 
While working with the deep-learning model, the number of neurons can be equal to the number of features involved after feature engineering and hidden-layers can be used according to your choice. For the activation function, we are using 'mse' and optimizer as adam. 

After performing descriptive statistics, predictive and inferential analysis, we can compare these two by measuring error metrics that include mean absolute error, mean squared error and root mean squared error.  We will also predict a price for new data using these two following models so that one can get the idea of deviation from the true price.

Features for DataSet 1:-
Feature Columns
id - Unique ID for each home sold
date - Date of the home sale
price - Price of each home sold
bedrooms - Number of bedrooms
bathrooms - Number of bathrooms, where .5 accounts for a room with a toilet but no shower
sqft_living - Square footage of the apartments interior living space
sqft_lot - Square footage of the land space
floors - Number of floors
waterfront - A dummy variable for whether the apartment was overlooking the waterfront or not
view - An index from 0 to 4 of how good the view of the property was
condition - An index from 1 to 5 on the condition of the apartment,
grade - An index from 1 to 13, where 1-3 falls short of building construction and design, 7 has an average level of construction and design, and 11-13 have a high-quality level of construction and design.
sqft_above - The square footage of the interior housing space that is above ground level
sqft_basement - The square footage of the interior housing space that is below ground level
yr_built - The year the house was initially built
yr_renovated - The year of the house’s last renovation
zipcode - What zip code area the house is in
lat - Lattitude
long - Longitude
sqft_living15 - The square footage of interior housing living space for the nearest 15 neighbors
sqft_lot15 - The square footage of the land lots of the nearest 15 neighbors

Features for DataSet 2:-
The data contains the following columns:
'Avg. Area Income': Avg. Income of residents of the city house is located in.
'Avg. Area House Age': Avg Age of Houses in the same city
'Avg. Area Number of Rooms': Avg Number of Rooms for Houses in the same city
'Avg. Area Number of Bedrooms': Avg Number of Bedrooms for Houses in the same city
'Area Population': Population of city house is located in
'Price': Price that the house sold at
'Address': Address for the house


Results Obtained for DataSet1:-
Price Predicted for a new household by Deep-Learning Model:- 287608.62$
Price Predicted for a new household by Linear Regression Machine-Learning Model:- 251823.61285049$
True-Price of a Household:- 221900.0000$

Explained_variance_score by Deep-Learning Model:- 0.7986445293855888
Mean_absolute_error by Deep-Learning Model:- 103250.24837902682
Rootmean_squared_errorby Deep-Learning Model:- 166651.8092635992

Explained_variance_score by Linear Regression Machine-Learning Model:- 0.6951152537006628
Mean_absolute_error by by Linear Regression Machine-Learning Model:- 123998.57212893506
Rootmean_squared_errorby by Linear Regression Machine-Learning Model:- 201080.55278529544

So,the overall performance of deep-learning model looks better since it's variance score is close to 0.8 while variance score of linear regression model is 0.7 and that is because of the hidden-layers role,adam optimizer in order to update weights and learning rate. But the true price is nearer to the value predicted by machine learning model, so it depends on the domain knowledge and context of the problem to decide which algorithm is better.



Results Obtained for DataSet2:-
Price Predicted for a new household by Deep-Learning Model:- 1258693.8$
Price Predicted for a new household by Linear Regression Machine-Learning Model:- 1225941.63882637$
True-Price of a Household:- 1059033.5578701235$

Explained_variance_score by Deep-Learning Model:- 0.8736528317018113
Mean_absolute_error by Deep-Learning Model:- 101834.50999175698
Rootmean_squared_errorby Deep-Learning Model:- 127143.77013354731

Explained_variance_score by Linear Regression Machine-Learning Model:- 0.9178179926151777
Mean_absolute_error by by Linear Regression Machine-Learning Model:- 82288.22251914963 
Rootmean_squared_errorby by Linear Regression Machine-Learning Model:- 102278.82922291271

So, the overall performance of the linear regression model looks better since its variance score is close to 0.92 while the variance score of the deep-learning model is 0.87 and that is because of the number of features involved in deciding the price of a house is less as compared to the previous dataset. And the true price is nearer to both the values predicted by the following models, so in this particular case, one can use any of the models.
