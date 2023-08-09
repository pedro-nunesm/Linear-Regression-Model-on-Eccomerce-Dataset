# Linear Regression Model on Eccomerce Database

![](img/Eccomerce%20image.jpg)

### The goal of this project is help an Eccomerce to make a better investment decision, seeking a greater amount spent annually per customer.
### For this, I will use the Linear Regression Machine Learning model.


## 1- Business Problem
I'm supposedly helping out an e-commerce company based in New York City that sells clothes online, but also has in-store style and apparel consulting sessions. Customers walk into the store, have sessions/meetings with a personal stylist, then go home and order from a mobile app or website for the outfit they want.


The company is trying to decide whether to focus its efforts on mobile apps or its website. And for that, I'll implement a Machine Learning model to make the best decision based on data.

The dataset has information about:

**E-mail, Adress, Avatar, Avg. Session Length, Time on App, Time on Website, Length of Membership and Yearly Amount Spent** 





## 2- Solution (Step by step)
 **Step I** - Import Libraries;
 
 **Step II** - Load dataset (provided by ASIMOV ACADEMY);
 
 **Step III** - Analyze how the data is distributed;
 
 **Step IV** - Find correlation between the variables .
 
 **Step V** - Implement the Linear Regression Model
 
 **Step VI** - Test the prediction and compare with data test;
 
 **Step VII** - Evaluate the model using using metrics to measure errors;
 
 **Step VIII** - Make a conclusion


## 3- Insights
 ### **3.1 - Correlation between variables** 
  - First of all, i analyzed the dataset and identified 3 numeric variables that could be correlated with the Yearly Amount Spent.
  - So i used Seaborn graphs to indetifies in the beggining
   ![](img/Time%20on%20Web%20x%20Yearly%20Amount%20Spent.png)
     **Almost no Correlation**
   ![](img/Time%20on%20App%20x%20Yearly%20Amount%20Spent.png)
    **Slightly linear correlation**
   ![](img/Pairplot%20general.png)

  - Using Pairplot, its easy to see a linear correlation between Length of Membership and Yearly Amount Spent.
   ![](img/Linear%20Regression.png)

### **3.2 - Linear Regression Model**
 - To begin, i separate dataset between X (Numeric Variables) and Y(Year Amount Spent)
 - So i used Sklearn to create X_train, X_test, Y_train, Y_test
 - The objective was to use the Trainning Dataset to train the Linear Regression Model, and, after this, use the Test Dataset to measure the performance.
   
  ![](img/Comparing%20Prediction%201.png)
  ![](img/Comparing%20Prediction%202.png)

 - **Using the graphs, it is possible to see that the model behaved extremely satisfactorily, and made very accurate predictions based on data that it had not yet seen.**

### **3.3 - Measure Model Errors**
I calculated some error metrics:
  - Mean Absolute Error: **7.23**
  - Mean Squared Error: **79.81**
  - Root Mean Squared Error: **8.93**

 **The error is extremely low, considering that a divergence of less than $10 for a Yearly Amount Spent prediction.**
## 4- Conclusion



## 5- Next-Steps

