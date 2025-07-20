Chemical Reactor Yield Prediction Using Random Forest Regression

Project Description This project focuses on building a data-driven machine learning model to predict the yield percentage of a chemical reactor based on various operational parameters. The purpose is to assist in optimizing chemical processes by estimating the reactor output before actual production, which saves time, resources, and cost.

Dataset Overview The dataset was provided in a CSV file named chemical_reactor_data.csv. It contained several numerical input features representing reactor conditions such as temperature, pressure, concentration, and flow rates. The target variable was the yield_percent, representing the efficiency or output percentage of the chemical reaction.

Step by Step Implementation

Data Preparation The dataset was loaded using the pandas library. The target column yield_percent was separated from the input features. No missing values or categorical encoding steps were shown, suggesting the dataset was clean and numerical.

Feature and Target Variables The input features were stored in a variable named X and the target output yield_percent was stored in a variable named y.

Train-Test Split The data was split into training and testing sets using the train_test_split function from the sklearn library. Eighty percent of the data was used for training the model, and twenty percent was used for testing. A random state of forty two was used to ensure reproducibility of results.

Model Selection and Training A Random Forest Regressor was chosen for its ability to handle complex data relationships and reduce overfitting. The model was initialized with one hundred estimators and trained on the training data.

Prediction After training, the model was used to predict the yield on the test dataset. These predicted values were stored in a variable named y_pred.

Model Evaluation Two key evaluation metrics were used

Mean Absolute Error This measures the average magnitude of the errors between predicted and actual values. The lower the value, the better the model.

R Squared Score This measures how well the model explains the variability of the target variable. A value closer to one indicates a better fit.

Model Output

Mean Absolute Error was approximately 1.64

R Squared Score was approximately 0.96

This means that on average, the model’s prediction deviated by only about one point six four percent from the actual yield, and it could explain about ninety six percent of the variation in the yield percentage.

Visualization

A scatter plot was generated using matplotlib to compare actual versus predicted yield values. The x-axis represented the actual yield percentages while the y-axis represented the predicted yield percentages. The points on the plot were mostly aligned along the diagonal line, showing that the predictions closely matched the actual values.

The plot was saved as an image file named yield_prediction_plot.png for reporting and documentation purposes.

Conclusion

The project successfully demonstrated the application of machine learning in chemical process optimization. The Random Forest Regressor achieved high accuracy with minimal error, making it a reliable model for predicting reactor yield. This approach can be extended to real-world industrial settings for predictive analysis, operational efficiency, and proactive decision-making in chemical manufacturing.

Skills and Technologies Used

Python Programming

Data Analysis with pandas

Machine Learning with scikit-learn

Model Evaluation and Metrics

Data Visualization using matplotlib

Regression Modeling
![Yield Prediction Plot](yield_prediction_plot.png)
