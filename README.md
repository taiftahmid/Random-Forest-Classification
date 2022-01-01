# Random-Forest-Classification

A Random Forest Model for predicting the key audiences to show ads in a social network. 

The dataset has the following features:
- User ID

- Gender
- Age

- Estimated Salary

- Purchased 

Using these features, the model predicts which audiences the ads will be relevant to. 

The feature dimensionality reduction was also done using Kernel PCA to increase the accuracy of the model

# Results and Discussion:

![alt text](https://github.com/taiftahmid/Random-Forest-Classification/blob/master/random_forest_training.png)

The green portion represents the users who bought the product viewed in the ads and the red portion represents the users who didn't. This model has learned the optimum line that seperates users who are prone to buying the product. 

For any new user, the model will simply check the position of the new user in the graph and predict whether the user is a key customer or not. 

The following figure shows the predictions made by the model from new users. (Test Set)

![alt text](https://github.com/taiftahmid/Random-Forest-Classification/blob/master/random_forest_test.png)

For this dataset, increasing the number of estimators to even to 100 did not improve the accuracy of the dataset and as a result, the n_estimators was kept to 10. 

The Random Forest Classification model works by making splits in the dataset and brings out new information. But unfortunately the splits also made the visualisation of the 
results a little unreadable as well. Will work on making a better visual plot in the future 

The accuracy of the model was 91%
