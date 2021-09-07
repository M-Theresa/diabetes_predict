## Project Overview
This project uses K-Nearest Neighbors classifier to predict if a patient is likely to develop diabetes based on certain diagnostic measurements including BMI, insulin level etc.

## Resources Used
Packages: **pandas, numpy, sklearn, matplotlib, seaborn**<br/> 
Dataset: The dataset used in the project is `diabetes.csv`. This dataset is originally from the National Institute of Diabetes and Digestive and Kidney Diseases. 

## Model Building and Evaluation
Plot the histogram plot of each feature and divide into two groups: diabetes and no diabetes. The histogram shows how each feature correlates to the possibility of developing diabetes.For example: <br/>

![distribution Plot](https://github.com/M-Theresa/diabetes_predict/blob/16273723fab63580d51bbd600aa50391720bb346/eda_plot.png)

Use `StandardScaler` to normalize the dataset and plot the distribution plot of orginal vs normalized dataset.<br/>
Use `KNeighborsClassifier` and choose k from 1 to 20. Calculate the accuracy score for different k values. The accuracy plot is shown below:

![accuracy Plot](https://github.com/M-Theresa/diabetes_predict/blob/2fd90215a9b7f6d692d3e75dfc416e98bb4dc31b/accuracy_score.png)

Based on the graph, the k value with the highest accuracy score is (12+1). Plot the distribution of the predicted outcome vs test data for using k=13. 

![accuracy Plot](https://github.com/M-Theresa/diabetes_predict/blob/16273723fab63580d51bbd600aa50391720bb346/predict_outcome.png)
