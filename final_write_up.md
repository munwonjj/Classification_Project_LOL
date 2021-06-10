# **PREDICTING WIN/LOSS RATE OF GAME - LEAGUE OF LEGENDS**

## ABSTRACT 

The goal of this project is to try to accurately predict the win/loss rate of the ranked match games in a game called League of Legends and potentially
suggest which feature may be relatively more important that impacts the win/loss of the game. The dataset consists of 26,000+ rows of Challenger data from 
[Kaggle](https://www.kaggle.com/gyejr95/league-of-legends-challenger-ranked-games2020/). The project utilizies various classification algorithms such as KNN,
Logistic Regression, and Random Forest. Although Random Forest produced the best result, Logistic Regression was selected as the final model to interpret 
the coefficients of the various features.

## DESIGN

Feature selection and hyperparameter tuning was used in the model. Among the 50 features, half of the features were dropped because only one side of the team
was needed to be analyzed (Blue team was selected).KNNClassifier and GridSearchCV was used to explore the data at first to find the best parameter for the model.

## Data

Data consists of 26,000+ observations with 50 features. 50 features were then reduced to 25 features to only explore the Blue side of the team. Among the 25
features, 6 features including our target variable blueWins were categorical variable. Some features include number of kills, assists, or objectives such as
dragon or Baron secured throughout the game. These dataset comes from ranked game of Challenger tier.

## Algorithms/Tools

* Python(Pandas + Numpy) for data manipulation
* sklearn package for Logistic Regression model (final chosen model)
* F1, AUC/ROC scores for classification metric
* matplotlib for visualizations
* Confusion Matrix to convey result

## Communication

Confusion Matrix was used along with ROC/AUC graph to compare different models.

1. Logistic Regression Confusion Matrix :

![Logistic Regression Confusion Matrix](https://github.com/munwonjj/Classification_Project/blob/main/confusion_matrix_graph.png)

2. ROC/AUC curve for 3 different models :
![curve](https://github.com/munwonjj/Classification_Project/blob/main/all_ROC_curves.png)


