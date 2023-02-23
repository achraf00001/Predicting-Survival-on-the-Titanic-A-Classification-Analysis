# Predicting-Survival-on-the-Titanic-A-Classification-Analysis 

Classification:
In this classification setting, we use a Titanic data set,it is a subset of a data set from https://www.ka
ggle.com/c/titanic. The Titanic data set contains information of 891 passenger with 11 variables (survived,Name,Pclass , Sex , Age , SibSp , Parch , Fare ,Embarked ,ticket, cabin). We will use this data
in order to create a model that can predict if passengers are going to survive or not, using two different
classifications method logistic regression and linear discriminant analysis.

data description:

survived ==> there are two levels 0 means the passanger did not survived and 1 means that the passenger
did survive. 0 = No, 1 = Yes.
pclass ==> Ticket class, there are three levels 1 means the firs class, 2 means the second class , 3 means
the third class. 1 = 1st, 2 = 2nd, 3 = 3rd
sex ==> Sex(gender) male or female
Age ==> Age in years.
sibsp ==> number of siblings or spouses aboard the Titanic.
parch ==> number of parents or children aboard the Titanic.
ticket ==> Ticket number.
fare ==> Passenger fare.
cabin ==> Cabin number.
embarked ==> Port of Embarkation. there are tree levels: C = Cherbourg, Q = Queenstown, S = Southampton. 

First we remove the missing values from our data in order to make our study easier. since the cabin column
has a lot of missing values we are going to remove this column from the data, also we remove the missing
values for Age and embarked.

Then we split the data into training and test set. The training set should be used to build our machine
learning models. in other words we are going to create a model based on our training data then we test our
model on the test data.The test set should be used to see how well our model performs on unseen data.For
each passenger in the test set, we use the model that we trained to predict whether or not they survived the
sinking of the Titanic.
