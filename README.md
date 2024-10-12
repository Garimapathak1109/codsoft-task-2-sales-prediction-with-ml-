# codsoft-task-2-sales-prediction-with-ml-
# Sales Prediction Project Using Machine Learning

## Project Overview
This project uses machine learning to predict sales based on advertising expenditure data across three channels: TV, Radio, and Newspaper. By analyzing feature importance and comparing models, the goal is to identify the most effective channels for advertising and optimize budget allocation to maximize sales outcomes.

## Analysis Summary and Findings

### 1. Feature Impact
   - The analysis revealed that **TV and Radio advertising** expenditures have the strongest correlation with sales, indicating they are key drivers of revenue.
   - **Newspaper advertising** had a smaller impact, suggesting that reallocating budgets toward TV and Radio may improve advertising ROI.

### 2. Model Comparison
   - Three machine learning models were tested: **Linear Regression**, **Decision Tree**, and **Random Forest**.
   - Among them, the **Random Forest model** outperformed the others, achieving a higher R-squared score and a lower Mean Squared Error (MSE), which shows its ability to capture complex relationships in the data.

### 3. Cross-Validation and Model Stability
   - Cross-validation was applied to test model stability, and results showed **consistent R-squared scores** across multiple data folds for the Random Forest model.
   - This stability indicates that the Random Forest model generalizes well to new data and is less sensitive to variations in the training dataset.

### 4. Hyperparameter Tuning
   - Using **GridSearchCV**, we optimized the Random Forest model's hyperparameters, leading to an even stronger R-squared score on the test set.
   - This tuning confirmed the model's accuracy, enhancing its ability to make reliable predictions.

### 5. Final Model Performance
   - The final Random Forest model, after tuning, demonstrated strong predictive capability on the test set with a high R-squared value, reinforcing its effectiveness for forecasting sales based on advertising expenditures.

## Recommendations

### Advertising Strategy Optimization
   - **Focus on TV and Radio Advertising**: Based on feature importance, a more targeted advertising approach is recommended, with increased budget allocations toward TV and Radio channels. This strategy is expected to yield higher returns on advertising spend.
   - **Deploy the Optimized Random Forest Model**: The fine-tuned Random Forest model can now reliably forecast future sales based on advertising expenditure, helping businesses make data-driven decisions for budget allocation.

## Getting Started

### Prerequisites
To run this project, you’ll need the following Python libraries:
```bash
pip install pandas seaborn matplotlib scikit-learn joblib
