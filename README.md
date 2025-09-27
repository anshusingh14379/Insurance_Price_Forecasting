# Insurance Price Forecasting Project (Python)
This project is an end-to-end machine learning solution designed to predict insurance charges based on client demographics and health-related features. We utilize Python for data processing, exploratory data analysis (EDA), and model building using Linear Regression, Random Forest, and Polynomial Regression. This project is ideal for data analysts and ML enthusiasts looking to develop skills in predictive modeling, data visualization, and feature engineering

### Project Steps
#### 1. Set Up the Environment
    - Tools Used: Visual Studio Code (VS Code), Python, Jupyter Notebook
    - Goal: Create a structured workspace and organize project folders for smooth development and data handling.

#### 2. Load and Explore Dataset
    - Dataset: insurance.csv (contains age, sex, BMI, number of children, smoking status, region, and insurance charges)
    - Python Libraries: pandas, numpy, matplotlib, seaborn
    - Steps:
        - Load data into a Pandas DataFrame
        - Inspect the first few rows (.head())
        - Check summary statistics (.describe()) and data types (.dtypes)
        - Identify missing values (.isnull().sum())

#### 3. Data Visualization
    - Visualize relationships between features and insurance charges using:
    - Scatter plots (age vs charges, smoker vs non-smoker)
    - Boxplots (children, smoker)
    - Distribution plots and log-transformed distributions
    - Correlation heatmaps for feature interactions
    - Bar charts for region-wise total charges

#### 4. Model Building
    - Models Used:
        - Linear Regression – baseline predictive model
        - Random Forest Regressor – handles non-linear relationships
        - Polynomial Regression – captures polynomial relationships between features
      
    - Steps:
        - Split data into training and testing sets (train_test_split)
        - Train models on training data
        - Make predictions on test data
        - Evaluate using R², MAE, and MSE metrics

#### 5. Model Evaluation

    | Model                 | R² Score | MAE  | MSE      |
    | --------------------- | -------- | ---- | -------- |
    | Linear Regression     | 0.75     | 3000 | 15000000 |
    | Random Forest         | 0.88     | 2000 | 8000000  |
    | Polynomial Regression | 0.80     | 2500 | 12000000 |
    - Insights:
        - Random Forest achieved the highest predictive accuracy.
        - Smoking status, BMI, and age are the most important features influencing insurance charges.

#### 6. Feature Importance
    - Random Forest feature importance plotted to identify key factors affecting insurance charges:
      - Most Important: Smoker, BMI, Age
      - Moderately Important: Children, Sex
      - Least Important: Region

#### 7. Project Structure

    insurance-price-forecasting/
    │
    ├── data/                     # Raw dataset
    ├── notebooks/                # Jupyter notebook with EDA, modeling, and visualization
    ├── scripts/                  # Optional: Python scripts for model training
    ├── images/                   # Plot images for README
    ├── README.md                 # Project documentation
    ├── requirements.txt          # Python dependencies
    └── .gitignore                # Files to ignore

#### 8. Results and Insights
    - Age & Smoking: Smokers incur significantly higher charges.
    - BMI Influence: Higher BMI leads to higher insurance costs.
    - Children & Region: Minor effect on insurance charges.
    - Best Model: Random Forest Regressor provides the most accurate predictions.

#### 9. Requirements
    - Python 3.8+
    - Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
    - code: pip install pandas numpy matplotlib seaborn scikit-learn
