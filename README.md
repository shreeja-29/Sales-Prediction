# 📈 Sales Prediction

## Overview

The **Sales Prediction** project is designed to forecast product sales using historical sales data and machine learning techniques. By analyzing various factors—such as advertising spend, promotions, and customer segmentation—this model helps businesses uncover key drivers of sales growth and optimize their marketing strategies.

## Objectives

- **Forecast Sales:** Build a predictive model that estimates product sales based on historical data.
- **Factor Analysis:** Examine the impact of variables like advertising expenditure, promotional activities, and customer segmentation on sales performance.
- **Robust Data Handling:** Manage missing values, detect and address outliers, and apply feature scaling to ensure optimal model performance.
- **Performance Evaluation:** Use appropriate metrics and visualizations to evaluate and fine-tune the model.

## Methodology & Approach

### 1. Data Collection & Exploration
- **Dataset:** The project uses the `car_purchasing.csv` dataset, which contains historical sales-related data.
- **Initial Exploration:** Detailed exploratory data analysis (EDA) is performed to understand the distribution of features, detect missing values, and identify outliers.

### 2. Data Preprocessing
- **Missing Value Imputation:** Rows or columns with missing data are handled appropriately to maintain data integrity.
- **Outlier Detection:** Outliers are identified (using methods like IQR-based filtering) and removed to prevent skewing the model.
- **Feature Scaling:** Numerical features are standardized using techniques like StandardScaler to ensure uniformity across features.
- **Data Engineering:** Categorical variables (e.g., promotions, customer segmentation) are transformed using one-hot encoding or label encoding.

### 3. Model Selection & Training
- **Algorithm Choice:** A Random Forest Regressor is utilized for its robustness and capacity to model complex, non-linear relationships.
- **Training:** The preprocessed and scaled data is split into training and testing sets. The model is then fitted on the training data.
  
### 4. Evaluation & Analysis
- **Performance Metrics:** The model’s performance is evaluated using:
  - **Root Mean Squared Error (RMSE)**
  - **R² Score**
  - **Custom Accuracy Metrics** (percentage of predictions within an acceptable error margin)
- **Visualizations:** Scatter plots, residual histograms, and bar charts are generated to visualize results and analyze error distributions.
  
### 5. Business Impact
- **Actionable Insights:** The model’s output assists in identifying critical marketing levers, enabling businesses to adjust their advertising spends and promotional strategies for improved sales growth.
  

## How to Run the Project

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/shreeja-29/Sales-Prediction.git
   cd Sales-Prediction
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare the Dataset:**
   - Ensure that the `car_purchasing.csv` file is placed in the `data/` folder.

4. **Run the Model:**
   - Launch the main script:
     ```bash
     python src/sales_prediction.py
     ```
   - Alternatively, open and run the Jupyter Notebook in the `notebooks/` folder for an interactive experience.

## Results & Insights

When executed, the project offers:
- **Detailed Evaluation:** RMSE, R² Score, and custom accuracy metrics to assess the model’s performance.
- **Visualization:** Clear graphical representations of prediction performance and error distributions.
- **Strategic Insights:** Actionable recommendations for refining marketing strategies based on sales forecasting outcomes.
