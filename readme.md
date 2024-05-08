# upGrad Course 8:

## Capston project:

### Credit card fraud detection

Dataset:
[Kaggle link for Data](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)


Reference Learning:

[The Use of Principal Component Analysis to Mask Sensitive Data in Machine Learning](https://medium.com/lizuna/beacon-the-use-of-principal-components-analysis-to-mask-sensitive-data-in-machine-learning-7904b01445d0)


### Summary

The project pipeline can be briefly summarized in the following four steps:

●     **Data understanding**: Here, you need to load the data and understand the features present in it. This would help you choose the features that you will need for your final model.
 

●     **Exploratory data analytics (EDA)**: Usually, in this step, you need to perform univariate and bivariate analyses of the data, followed by feature transformations, if necessary. For the current data set, because Gaussian variables are used, you need not perform Z-scaling. However, you can check if there is any skewness in the data and try to mitigate it, as it might cause problems during the model building phase.

Now, let’s discuss why skewness may be an issue while modeling. Some of the data points in a skewed distribution toward the tail may act as outliers for the machine learning models that are sensitive to outliers; hence, this may cause a problem. Also, if the values of any independent feature are skewed, depending on the model, skewness may affect model assumptions or may impair the interpretation of feature importance.

●     **Train/Test split**: Now, you are familiar with the train/test split that you can perform to assess the performance of your models with unseen data. Here, for validation, you can use the k-fold cross-validation method. You need to choose an appropriate k value so that the minority class is correctly represented in the test folds.
 

●     **Model building / hyperparameter tuning**: This is the final step where you can try different models and fine-tune their hyperparameters until you get the desired level of performance.