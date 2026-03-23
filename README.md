# Lab4_Pandas_Boston-Housing-Prediction
Boston Housing price prediction using Pandas &amp; ML. Data preprocessing, feature analysis, and regression modeling to estimate housing values with clear insights.

Overview: 
This lab explores the Boston Housing dataset to predict the median value of owner-occupied homes.
We perform data exploration, visualization, and apply multiple regression algorithms: Linear Regression, Decision Tree Regression, and Random Forest Regression.
The goal is to compare performance across models using R² and RMSE, interpret results, and highlight trade-offs between accuracy and interpretability.

Step 1: Load Required Libraries
numpy, pandas
matplotlib, seaborn (visualizations)
scikit-learn (train_test_split, LinearRegression, DecisionTreeRegressor, RandomForestRegressor, metrics)

Load the Data:
Dataset: Boston Housing Dataset (506 rows, 14 columns).

Target variable: MEDV (Median value of homes in $1000s).

Features include: crime rate (CRIM), average rooms (RM), age of buildings (AGE), tax rate (TAX), pupil-teacher ratio (PTRATIO).

Data Exploration:
Dataset shape: (506, 14)

No missing values detected.

Summary statistics show wide variation in crime rate, rooms per dwelling, and housing prices.

Data Visualization
Histograms & Boxplots: Distribution of housing prices (MEDV), crime rate (CRIM).

Scatter Plots:

AGE vs MEDV (older buildings → lower prices).

RM vs MEDV (more rooms → higher prices).

CRIM vs MEDV (higher crime → lower prices).

Bar Plots: Average housing price by accessibility to radial highways (RAD), zoning (ZN).

Correlation Heatmap: Strong positive correlation between RM and MEDV; negative correlation between LSTAT (lower status population %) and MEDV.

Train-Test Split:
Training set: 70% (354 samples).

Test set: 30% (152 samples).


Step 6: Applying Machine Learning Algorithms:

Linear Regression
Intercept: ~31.63

RMSE: 4.64

R²: 0.71

Interpretation: Moderate fit, interpretable coefficients.

Decision Tree Regression:
RMSE: 3.45

R²: 0.84

Interpretation: Captures non-linear relationships, better accuracy, risk of overfitting.

 Random Forest Regression
RMSE: 3.10

R²: 0.87
Interpretation: Best performance, balances accuracy and generalization.

Conclusion:
Linear Regression: Provided a baseline with moderate accuracy and interpretability.

Decision Tree Regression: Improved accuracy by modeling non-linear relationships.

Random Forest Regression: Achieved the highest accuracy and lowest error, making it the most reliable model for this dataset.

Overall, ensemble methods like Random Forest outperform simpler models, while visualizations highlight key feature relationships (RM, LSTAT, CRIM).


