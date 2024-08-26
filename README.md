# Tecnologico de Monterrey Project
This project is part of  a test for a Research Programmer and Data Scientist position at the 
Decision Sciences Research Center at Tecnologico de Monterrey. 

The project consists of 5 questions about CO2 emissions worldwide and studies the impact of many variables.
## Package
pip install numpy pandas matplotlib seaborn wbgapi scikit-learn plotly -U kaleido


## Question 1
This program downloads the data using the World Bank Data Library considering many economic and environmental indicators.

Then clean and substitute the NaN-values using a k nearest neighbor algorithm.<br>
The last part shows the correlation between the economy and environmental variables.<br>
This ipython returns the csv file of the data obtained, and the correlation between the variables.<br>

![](https://github.com/alhan12/Tec_project/blob/main/correlation.png) 
## Question 2
This program makes a linear regression assuming that CO2 emissions are the dependent variable and splits the data into training and testing sets.<br>
Suppose that there is an increase in GDP, and then apply and analyze the results.<br>
And returns the information into an interactive graph comparing the projected and current emissions.
![](https://github.com/alhan12/Tec_project/blob/main/a.png)
![](https://github.com/alhan12/Tec_project/blob/main/b.png)

However, the Linear regression is not valid, since the r^2 value is negative, and the scatter plot shows a non-linear behavior.
![](https://github.com/alhan12/Tec_project/blob/main/CO2%20emissions%20errors.png) 

## Question 3
This program adds more data into the csv file using the World Bank Data Library considering new environmental indicators.<br>
Again, clean the data and add NaN values using the k nearest neighbor algorithm to sustain the values.<br>
Now, since the EV adoption was not available in the WBD, I used a similar variable (renewable energy percentage) since there is a negative correlation concerning CO2 emissions.<br>
I used and trained a Linear regression and used it to predict what would happen to CO2 emissions if the renewable energy percentage increased. <br>
The program returns the interactive plots<br>

![](https://github.com/alhan12/Tec_project/blob/main/c.png)

Since there is a new condition, the emissions should be always positive or at least zero, though many predictions do not hold this condition, so I cleaned the results and plotted only the countries where Linear regression is valid.
![](https://github.com/alhan12/Tec_project/blob/main/d.png)
The linear regression is not valid since the r^2 value is negative, and the data show a non-linear behaivior.
![](https://github.com/alhan12/Tec_project/blob/main/CO2%20emissions%20errors%20(renew).png)

## Question 4
This program classifies the data through a binary variable and uses a Random Tree classificator. It trains the algorithm with the data that we have collected in question 3.
Here is the importance of features in CO2 emissions reduction.
![](https://github.com/alhan12/Tec_project/blob/main/features.png)


## Question 5

This final part assumes that in a country where the renewable energy percentage is less than 10% and increases the percentage by 50%, what would happen?<br>
To predict the probability we use the classifier trained in the last problem, and the results are plotted in the interactive plot
![](https://github.com/alhan12/Tec_project/blob/main/e.png)

The blue points represent the countries where there is a high likelihood of decreasing their CO2 emissions while the red points represent the countries where is not possible.<br>
So the plot shows that most than half of the countries could decrease their CO2 emissions.
