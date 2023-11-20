# FilmRecommendationAndIMDBRatingPrediction
# Project Overview
This project entails two primary objectives. Firstly, the goal is to develop a recommendation system that allows users to discover movies similar to those they've previously watched. The second objective involves creating a system to predict IMDb ratings for upcoming movies. The initial stages involved data merging and cleaning, followed by exploratory data analysis (EDA) and correlation analyses using Spearman and Pearson methods to identify relevant features.

To achieve the recommendation system, two unsupervised machine learning algorithms—Cosine Similarity and K-means clustering—were implemented. For IMDb rating prediction, three supervised machine learning algorithms were employed. Among them, two were classification algorithms, namely KNN and Random Forest classification. The subsequent step involved assessing and determining the most effective algorithms for both the recommendation and prediction systems.
Code and Resources Used
- ***Python Version:*** 3.8
- ***Packages:*** pandas, numpy, sklearn, matplotlib, seaborn
- ***Dataset:*** Netflix: https://www.kaggle.com/shivamb/netflix-shows IMDb data: https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset

The project began with the loading and merging of two datasets, 'netflix_titles.csv' and 'IMDb movies.csv,' to facilitate movie and show recommendations. Data cleaning involved dropping duplicates and handling null values. Exploratory data analysis included top ratings, pie-charts, bar-graphs, and box plots illustrating content distribution based on age, ratings, and genre.

Encoding was employed to convert string columns into integers using Sklearn's OrdinalEncoder. Correlation analysis using Pearson's and Spearman's methods visualized the connections between numerical attributes. The machine learning models comprised unsupervised models for the recommendation system and supervised models for IMDb rating prediction.

For unsupervised models, K-means clustering utilized the elbow method and PCA for dimensionality reduction, yielding effective clusters. Cosine Similarity, based on a bag of words approach, created a similarity matrix for recommendations.

Supervised models included Random Forest, KNN, and Linear Regression for IMDb rating prediction. Hyperparameter tuning and feature importance improved Random Forest's accuracy to 62%, outperforming KNN and Linear Regression. Accuracy, MSE, MAE, and rMSE were compared, with Random Forest standing out.

In conclusion, both film recommendation and IMDb prediction systems demonstrated effectiveness to a certain extent. Random Forest proved superior in IMDb prediction, while cosine similarity outperformed K-means in the recommendation system. Linear regression also showed notable performance in rating prediction. Overall, the results indicate a successful implementation of the proposed algorithms.
