# Tec_project
This project is part of  a test for a Research Programmer and Data Scientist position at the 
Decision Sciences Research Center at Tecnologico de Monterrey. 

The project consist of 5 questions about the CO2 emission throughout the world and study the impact of many varaibles.
## Package
pip install numpy pandas matplotlib seaborn wbgapi scikit-learn plotly -U kaleido


## Question 1
This program downloads the data using the World Bank Data Library considering many economic and environmental indicators.

Then clean and substitute the NaN-values using a k nearest neighbor algorithm.<br>
The last part shows the correlation between the economy and environmental variables.<br>
This ipython returns the csv file of the data obtained, and the correletion between the variables.<br>

![](https://github.com/alhan12/Tec_project/blob/main/correlation.png) 
## Question 2
This program make a Linear regression assuming that CO2 Emissions are the dependent variable, split the data into training and testing set.<br>
Supossed that there is an increase in GDP and applies and analyses the results.<br>
And returns the information into a interactives graph comparing the projected and current emission.
![](https://github.com/alhan12/Tec_project/blob/main/a.png)
![](https://github.com/alhan12/Tec_project/blob/main/b.png)
## Question 3
This program adds more data into the csv file using the World Bank Data Library considering new environmental indicators.<br>
Again, clean the data and add NaN values using the k nearest neighbor algorithm to sustite the values.<br>
Now, since the EV adoption was not avaible in the WBD, I used a similar variable (renewable energy percentage) since there is a negative correlation respect to CO2 emissions.<br>
I used and train a Linear regression and use it to predict what would happen to CO2 emissions if the renewable energy percentage increase. <br>
The program returns the interactive plots<br>

![](https://github.com/alhan12/Tec_project/blob/main/c.png)

Since there is a new condition, the emissions should be always positive or at least zero, but many prediction does't hold this condition, so I cleaned the results and ploted only the countries what Linear regressions is valid.
![](https://github.com/alhan12/Tec_project/blob/main/d.png)
## Question 4
This program classifies the data through a binabary variable, uses a Random Tree classificator.
![](https://github.com/alhan12/Tec_project/blob/main/features.png)
## Question 5

