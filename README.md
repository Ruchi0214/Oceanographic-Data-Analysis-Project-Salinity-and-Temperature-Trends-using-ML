# Oceanographic-Data-Analysis-Project-Salinity-and-Temperature-Trends-using-ML
Problem statement: TO ANALYZE AND MODEL THE RELATIONSHIP BETWEEN SALINITY AND TEMPERATURE IN OCEANOGRAPHIC DATA USING MACHINE LEARNING TECHNIQUES”. Ocean salinity and temperature are two critical parameters that influence ocean circulation and climate patterns. Understanding the complex relationship between these variables can help predict future changes in the ocean's behavior.

The dataset used is sourced from the CalCOFI (California Cooperative Oceanic Fisheries Investigations) dataset, which includes historical oceanographic data. In this problem, we aim to build a predictive model using polynomial regression to predict temperature based on salinity values. Polynomial regression is employed because the relationship between salinity and temperature is often non-linear, and a simple linear model may not capture the complexity of the data.
DATA ARCHITECTURE AND FLOW:

![image](https://github.com/user-attachments/assets/8c6b8f43-a3b7-4ae4-8eb8-577e9b36c976) 
Functionality with perspective library 
1.	Data Ingestion 
•	The project begins by loading a dataset (bottle.csv) containing oceanographic data, focusing on two key variables: Salinity (Sal) and Temperature (Temp).
•	The code selects the first 250 rows and cleans the data by removing any missing values to ensure accurate model performance.

2.	Data Visualization 
•	Once the data is organized, we need to see patterns. Seaborn is a data visualization library that allows to create visually appealing charts. Before modeling, the code uses Seaborn to plot the relationship between salinity and temperature.
![image](https://github.com/user-attachments/assets/988fc465-f57c-4133-863e-7aef04ab95d9)

3.	Feature Engineering
•	To capture complex relationships, the salinity feature is transformed into polynomial features of degree 3 using PolynomialFeatures from Scikit-learn. This allows the model to consider non-linear interactions between salinity and temperature.
![image](https://github.com/user-attachments/assets/3a118edf-cfa7-45f1-b8c9-1159a6581ddd)

4.	Model Evaluation
•	Prints the training score of the model and predicts temperature values for the test data.

5.	Model Deployment
•	Plot the actual data and predicted curve using matplotlib.
•	Visualize the results to evaluate the performance of the model.

![image](https://github.com/user-attachments/assets/e909651c-72a8-4cdf-9f83-b38c89c060e6)

**RESULTS:**
•	The polynomial regression model performed quite well, as seen by its 91% (0.919) score. The result obtained in machine learning usually indicates how well the target variable's variation is explained by the model.

•	With an R² of 0.919, the model based on the salinity measurements can account for 91.9% of the variation in temperature. The more closely the model's predictions match the actual data, the closer the R2 value is to 1. In this instance, the model's high predictive power is indicated by its 91% score.

•	Accuracy - With a 91% score, the model is often able to forecast temperature based on salinity. Because of its high degree of accuracy, the model may be used to real-world problems including environmental monitoring, oceanographic research, and marine science predictive analytics.

•	The choice of polynomial degree was important in this investigation. Non-linear behaviors are frequently seen in real-world environmental phenomena, such as the interplay between temperature and salt in ocean water. It would have been too easy to express these variances with a linear model. Nevertheless, the regression model was able to represent curved connections and capture the highs and lows in the data by adding polynomial component

•	Practical Application - Many oceanographic research depends on an understanding of the link between salinity and temperature since these two variables affect a variety of biological and physical processes in the ocean. 


