# Risk-Analytics-In-Banking-Financial-Services


#Introduction

India has been ranked 5th in the list of countries with the highest Non - Performing Assets. It implies India possesses more defaulters each year regarding the subject’s ability to repay their loans. Noticeably this is an alarming figure and with the rise of Bank frauds, figured at high as 100 Crore per day. With this as our motivation, we’ve decided to work on a problem that suitably allows us to identify whether or not a bank can engage in business with a client based on their previous history. Using ML techniques taught, our project aims at creating an efficient model where we can appropri- ately find the right set of metrics from a diverse group of features that helps us in identifying whether a subject can repay their loan once taken.

#Data-set Description

The Dataset has been taken from Kaggle. The dataset is composed of two CSV files, application data.csv and previous application.csv. The application data.csv file has the Dimensionality of 307511 x 122 (rows x columns). It consists of 122 features that give the applicant’s current status in need of a loan. It contains all the information of the client at the time of application. The data is also concerning whether a client has had payment difficulties. The 2nd file has the Dimensionality of 1670214 x 37 (rows x columns), containing information about the client’s previous loan data. It includes whether the previous application had been approved, cancelled, refused, or unused. As a part of our interim goals, we built a united dataset that accounted for both the application data and the previous application data of the clients. We obtained the client IDs with the help of the SK ID feature. We’ve merged both datasets into one. So our united dataset is only limited to those IDs that match both datasets.

#Evaluation

We have merged both CSV files and appropriately split training and testing sets in a 4:1 ratio. Since our dataset’s number of features has exceeded, we dropped some of the features that did not contribute much to the evaluation and have more null values than the data itself( see fig 8 ). Furthermore, we have applied dimensionality reduction and extracted only the necessary features using PCA (see fig 9) for best two principal components ). We calculated the explained variance ratio for all features and extracted those that contribute more towards better model training(see fig 1). After PCA modelling of our united dataset, we are left with a dataset having the final dimension of 291057 rows against 44 features. From fig 10, we can compare the distribution of class variable for unsampled and undersampled dataset. After undersampling our resultant data becomes 38040 x 44.

#Conclusion 371

Although XGBoost and MLP both resulting in the best models with highest scores with respect to other models with and without optimisation. However, the best model with maximum metric score was Multi Layer Perceptron with best metrics scores as :-.precision score: 0.811, recall score: 0.813, F1 score: 0.823 and accuracy score: 0.923.
