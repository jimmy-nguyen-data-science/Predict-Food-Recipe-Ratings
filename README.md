# Project: Predict Food Recipe Ratings from Food.com

## Completed: 16 August 2021 

## Collaborators 
- Jimmy Nguyen 
- [Jose Luis Estrada](https://github.com/jose-luis-estrada)
- Ashutosh Singh 


## Installation

Data Exploration and Modeling was all done in [Jupyter Notebook](https://jupyter.org/).

To clone this repository onto your device, use the commands below:

	1. git init
	2. git clone git@github.com:jimmy-nguyen-data-science/Predict-Food-Recipe-Ratings.git
  

## Project Objective
The purpose of this project is to compare different machine learning models that predict a consumers' rating based on their reviews on a recipe from Food.com

## Project Background 
Food.com is a website that allows users to share and copy kitchen recipes. Formerly known as Genius Kitchen, the company collected data covering 18 years of user interactions and uploads. The data used in this project were acquired from Kaggle.com, a Machine Learning and Data Science Community website. The data includes 180K+ recipes and 700K+ recipe reviews. The goal is to work with a regularized linear classifier (logistic regression) on text data. Then using cross-validation to fine tune over different hyper-parameters, such as the regularization term. Afterwards, to improve the baseline performance with feature engineering and selection. Lastly, compare the final model performance with the initial baseline performance.

### Methodology
- Obtain data
- Define purpose 
- Data exploration
- Baseline Model - Data preprocessing
- Baseline Model - Regularized Linear Classifiers
- Baseline Model - Tuning for Optimal Hyper-parameters
- Improving Model - Feature Engineering and Selection
- Improving Model - Tuning for Optimal Hyper-parameters
- Results and Model Performance Comparison
- Conclusion

### Technologies
- Python
- Powerpoint
- Word

## Baseline Model - Regularized Linear Classifiers 
The baseline model of choice is using a regularized linear classifier with stochastic gradient descent, while estimating the gradient of the log loss function at each sample at a time. As so, these regularized linear models would then be logistic regression models. These models are trained by varying between the absolute norm L1 and squared euclidean norm L2 as a regularizer to control overfitting. These penalties will be trained in conjunction with fine-tuning for the optimal learning rate, or alpha. The steps for searching for the optimal hyper-parameters include a pipeline to fit the stochastic gradient descent classifier with the log loss function, iterating between the L1 and L2 penalty over a list of alphas in the range of 0.0001 to 1000 with a step size of 0.1. The choice for performance metric is accuracy because this is a multi-class classification problem. Due to accuracy being a misleading performance metric, it is better to use K-folds cross validation as a better approximation of accuracy instead of a random training and test-set split.

## Machine Learning Models
- Regularized Linear Classifiers (Logistic Regression): Tuned for Penalized Methods and Learning Rate
- Other Baseline Models: Neural Networks and Random Forest


## Presentations and Reports
* [Final Report](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Reports/Final%20Report.pdf)
* [Python Code](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Code/Python/Python%20Code%20-%20PDF%20.pdf)

## Performance Results 

- Baseline Models - Validation Performance Table
![Baseline Validation Performance Table](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Data%20Visuals/Baseline%20Validation%20Performance%20Table.png)

- Baseline Models - Validation Performance Graph
![Baseline Validation Performance Graph](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Data%20Visuals/Baseline%20Validation%20Performance%20Graph.png)

- Improving Baseline Models - Validation Performance Table
![Final Validation Performance Table](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Data%20Visuals/Final%20Validation%20Performance%20Table.png)

- Final Model - Confusion Matrix

![Final Performance Confusion Matrix](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Data%20Visuals/Final%20Performance%20Confusion%20Matrix.png)

- Final Model - Performance Report

![Final Performance Report](https://github.com/Jimmy-Nguyen-Data-Science-Portfolio/Predict-Food-Recipe-Ratings/blob/main/Data%20Visuals/Final%20Performance%20Report.png)

## Original Data 
[Kaggle - Food.com Recipes and Interactions](https://www.kaggle.com/shuyangli94/food-com-recipes-and-user-interactions?select=RAW_recipes.csv)

## References
Shuyang, L. Food.com Recipes and Interactions. Kaggle.com. Retrieved 16 August 2021, from
https://www.kaggle.com/shuyangli94/food-com-recipes-and-user-interactions

