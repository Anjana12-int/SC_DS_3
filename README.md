
## Customer Purchase Prediction using Decision Tree Classifier

This project uses a Decision Tree Classifier to predict whether a customer will make a purchase or not based on demographic and behavioral data  from online shoppers.

# Dataset

* Name: `online_shoppers_intention.csv`
* Source: Kaggle
* Target Variable: `Revenue` (True = Purchase, False = No Purchase)
* Features:

  * Administrative, Informational, ProductRelated durations
  * BounceRates, ExitRates, PageValues
  * VisitorType, Weekend, Month
  * OperatingSystems, Browser, Region, TrafficType


 # Objective

Build a predictive model that can classify whether a visitor will make a purchase or not using their session behavior and other contextual attributes.


# Steps Performed

1. Data Preprocessing

   * Handled categorical variables (`Month`, `VisitorType`) using Label Encoding
   * Converted boolean values (`Weekend`, `Revenue`) to integers

2. EDA (Exploratory Data Analysis)

   * Correlation heatmap
   * Class distribution check
   * Feature importance visualization

3. Model Building

   * Decision Tree Classifier with GridSearchCV for hyperparameter tuning
   * Stratified train-test split
   * Cross-validation (5-fold) to evaluate generalization

4. Evaluation

   * Accuracy: \~89.6%
   * Precision/Recall/F1-score reported
   * Confusion Matrix plotted
   * Visualized the trained Decision Tree


 # Key Insights

* `PageValues`, `ProductRelated_Duration`, and `ExitRates` are top predictors of purchases.
* Returning visitors are more likely to buy than new users.
* High bounce rates negatively affect purchase likelihood.
* Purchases are higher in specific months, indicating seasonal shopping trends.


 # Business Recommendations

* Improve product-related page content to boost engagement.
* Focus marketing efforts on returning visitors.
* Use seasonal trends to plan promotions.
* Reduce bounce rates with better landing page experiences.


 # Technologies Used
* Python 
* Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

