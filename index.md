# You want to rent your apartment on Airbnb?

If you are interested in rent your home in Seattle this article is for you. I used real data from Airbnb to answer some questions that can be take it into account before you decide to rent your home. The variables selected for the study are: accommodates, bathrooms, bedrooms, superhost, number of reviews, the review score rating, the reviews per month and the neighborhoods.


## How are the prices of Airbnb rentals in Seattle?

Based on the sample the mean price of the rent is $129.28 in Seattle. The minimum rent is $20 and the maximum is $1000. In the graph below you can see the distribution of the prices of the Airbnbs in this city.

<img width="396" alt="Image01" src="https://user-images.githubusercontent.com/89614195/162023177-f3f87847-e6f0-407f-ab32-d17e9e52c02c.png">

Also we can see that there are 81 neighborhoods with homes listed in Airbnb in this city. The top 5 neighborhoods with the highest price in Seattle:

<img width="225" alt="Image02" src="https://user-images.githubusercontent.com/89614195/162023220-c2c94f8f-bdfe-4470-9bda-b4674cc31cd3.png">

While the neighborhoods with the lowest prices are these ones:

<img width="212" alt="Image03" src="https://user-images.githubusercontent.com/89614195/162023253-17984dc1-2535-4248-9018-c8d128551b06.png">

## Which variables correlate with the price of the rent?

The correlation between variables can be measure with the Pearson correlation coefficient. This coefficient can take values between -1 and 1, where -1 represents a perfect negative correlation, while 1 a perfect positive correlation. The results of the correlation matrix for the variables evaluated in this project are shown below.

<img width="672" alt="Image04" src="https://user-images.githubusercontent.com/89614195/162023307-ad509217-f8fb-44dd-9d4c-64faac6b620f.png">

As you can see in the correlation matrix the variables with positive correlation with the prices are: accommodates, bathrooms and bedrooms. The variables with negative correlation are: number of reviews and reviews per month. Meanwhile the superhost and the review score ratings have near no correlation with the prices.

## Can we predict the rent of your home?

The next point in this project consist in the creation of a model to predict the price of an Airbnb rental in Seattle using the variables of the sample. In this occasion I used a linear regression model. The R-squared in the train data was 0.533 and in the test data was 0.606, this represents that the model explains the 60.6% of the variability of the price in the test data. 

Another aspect that must be interpreted are the coefficients of the linear regression. Since the variables were normalize, it is possible to measure the impact of the variable in the price. The chart below shows the 20 variables with the greater coefficient of the model. As you can see the neighborhood seems to be one the most important indicator for the price of the Airbnbs in Seattle.

<img width="387" alt="Image05" src="https://user-images.githubusercontent.com/89614195/162023361-11ce9663-1fec-4c68-9574-8d4154e8ea81.png">

In this way we have answered the proposed questions with the use of the Airbnb database for the city of Seattle. Also we have create a model that can be used to predict the possible rental price for your home on Airbnb.
