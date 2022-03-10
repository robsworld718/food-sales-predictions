# food-sales-predictions
| Syntax | Description |
| Pyhton | Creating visualizations that reveal insight about the sales prediction data. This will help allow us to choose and fit the proper machine learning model for further predictive analysis  |

1. Cleaning the data involved identifying the data types, viewing where my missing values for respective collumns were.
2. Next I then decided to run value counts on the numerical columns I would need for my visualizations.
3. Once that process was completed ran a heatmap to view my column correlations.
4. I then checked the value counts of specific columns I would be using for my visualizations.
5. Created visualizations for the distributions of individual columns (single variate histograms and boxplots with descriptions)
6. In the next step I creeated Visualizations (Multi-variate scatterplots, histograms, barplots and boxplots) to further explain the correlating columns,
7. Before deploying models I split the data into train and test sets creating X and y variables, removing the unique column item identifier
8. Using the SciKitLearn library I was able to divide the data into numeric and categoerical data by employing imputers for object and number columns secting both aby way of mean and most frequent strategies to transform the data.
9. Next I handled the missing values with a Standard scaler and deployed a One Hot Encoder to create a binary colum for each column through tuples. This is a must before passing data through our models. Then made pipelines to combine the variables with the previously created processes and assigned column transformers to finalize the preprocessing. Applied changes to the training data.
10. The first model I chose was a linear regression model and combined it to the pipe created earlier, fitting it to only the training data.
11. Lastly for this model I then score the pipes for accuracy
12. Was not satisfied so I further evaluated the model with a few more regression metrics and still got low scores (R^2 0.5615527181926836
 RMSE 1139.107242220339)
13. Since the dataset had multiple categoerical variables I chose to use a decision tree model. Since I created the pre processing variables already, I only had to deploy the model after creating a new pipe, attaching the transformer and fitting it to the data.
14. I then evaluated the scores(X,y), the decision tree depths and got better results ( R^2 0.9168944665022553
 RMSE 495.930585049585)
15. I added a Randomn Forest model to increase scoring by way of the enssemble method through weaker bagged trees. This resulted in a randomn Forest model being scored at 93% on training data and 56% on testing data. There was too much variance between testing and training data.

![OTBEY](https://user-images.githubusercontent.com/77306280/151509212-77521056-46e2-4e53-9244-aacd96afe5cc.png)

Summary: After reviewing the data I was able to relay 2 things. From the visualizations 

- [x] Clean Data
- [x] Create Visualizations
- [x] Train and test data
- [x] Create and apply Linear Regression Model
- [x] Create and apply Decision Tree Model
- [x] Summary of findings

[https://github.com/robsworld718/food-sales-predictions/blob/main/Copy_of_food_sales_predictions.ipynb)
Please follow the link to view the code from the homepage. [^1]

