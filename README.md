# Neural_Network_Charity_Analysis

Click here for the machine learning and neural network code: [AlphabetSoupCharity](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb) | [AlphabetSoupCharity_Optimization](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimzation.ipynb)


## Overview of Analysis

The objective of this challenge is to help the Alphabet Soup Charity help decide which organizations to invest in. This was done by applying machine learning neural network techniques to develop a binary classifier that is capable of predicting whether these organizations would be successful with Alphabet Soup's investment.


## Results

### Data Preprocessing

Click here to view the data preprocessing code between cells 1 to 15: [AlphabetSoupCharity](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb)

 - the target for the model is the "Is_Successful" column
 - The feature for the model: Application Type, Affiliation, Classification, Use Case, Organization, Active Status, Income Amount, Special Considerations, and the Ask Amount.
 - The "EIN" and "Name" columns are variables that are not targets

### Compile, Train, and Evaluate

The first model I developed consisted of two hidden layers with the first layer having 8 neurons and the second layer having 5 neurons. The sigmoid activation feature was applied here. In my first attempt with this model, I acquired an accuracy score of 55 percent. Unfortunately, this falls well below our goal of 75 percent accuracy.

![First_model_attempt](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/Resources/First_model_attempt.PNG)


### Optimization

I executed three additional attempts of improving the accuracy score to 75 percent by optimizing the model:

 - The first optimization I dropped the "Special Considerations" column and sadly, my accuracy score decreased to 48 percent 
 - The second optimization I increased the neurons in both hidden layers and while I improved my overall accuracy score to 57 percent, we still fell far below the 75 percent
 - The third optimization I added a third hidden layer and unfortunately, my accuracy score dropped to 53 percent, well below the 75 percent.

#### Attempt 1

![Optimize_1](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/Resources/Optimize_1.PNG)

#### Attempt 2

![Optimize_2](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/Resources/Optimize_2.PNG)

#### Attempt 3

![Optimize_3](https://github.com/jzaragoza21/Neural_Network_Charity_Analysis/blob/main/Resources/Optimize_3.PNG)



## Summary

As pointed out by the analysis above, all of our model attempts failed to reach an accuracy score of 75 percent or more. The best attempt was when the amount of neurons increased in the first and second hidden layers, resulting in an accuracy score of 57 percent, slightly better than a coin flip. As a result, I would recommend to perhaps a support vector machine model as it is really fitted for classification and regression models. 
