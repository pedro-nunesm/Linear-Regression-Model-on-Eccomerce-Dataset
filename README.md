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

 ![](img/Normal%20Distribution.png)


**Finally, by creating a graph using only the error value (Real Values - Predictions), it is possible to visualize a normal distribution, which reiterates that the Linear Regression model worked very well for this dataset.**

### **3.4 - Checking the Coefficients**
#### Coeffeciet:

**Avg. Session Length	25.981550**

**Time on App	38.590159**

**Time on Website	0.190405**

**Length of Membership	61.279097**

## 4- Conclusion
After all the analysis and verification of the model, it is possible to conclude that, for Eccomerce, comparing only the variables Time on Web and Time on App, it is more beneficial to invest in measures to increase Time on App.

However, analyzing everything that was observed, the most appropriate measure for Eccomerce, aiming at an increase in the Yearly Amount Spent for each customer, is to invest in measures to build customer loyalty, since it is the Length of Membership that, in fact, has a positive linear relationship with an increase in sales.

Looking at the coefficients, the Length of Membership variable has a much greater weight. A one-unit increase in this variable averages growth of $61.27, while a one-unit increase in Time on App averages only $38.59 growth.

## 5- Next-Steps


