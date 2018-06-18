## Predicting vehicles sale using xgboost

Tan Li, litan1209@qq.com
EECS 349: Machine Learning, Northwestern University

### Abstract

The main purpose of this project is to use machine learning tools to predict the sale of vehicles based on their previous sale. Such topic could be meaningful in several ways. for example, as we are the dealer, knowing the possible trend of the total sale of different vehicles in the next few months could help us manage the stock better. Moreover, by knowing what kind of cars are being more popular among the customers, the manufacturer could spend more resource on designing and producing cars with similar properties. 

In this work, a popular ensemble model, xgboost is applied on features including the vehicle information such as height and weight as well as some context information like when the car is sold. The key of xgboost’s outstanding performance was studied. The xgboost model with best parameters could overrun the baseline (the average sale) by 18.6% on root-mean-square error(rmse). The xgboost offers a function named get_fscore(). By calling this function on the as-trained model, one can see which of the features are used most frequently on which the tree nodes split. In the dataset used in this work, features with highest importance are sale from past 3 months, on which month or year the car is sold and the quality and the height of the car. The sum of predict sale of each month and that of the true value are shown in figure 1.

![figure 1. The sum of predict sale of each month and that of the true value]
