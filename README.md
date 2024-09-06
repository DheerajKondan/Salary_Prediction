# Salary Prediction using Machine Learning

This project focuses on predicting salaries for various job roles using machine learning models. The dataset includes several job-related features like job title, salary estimates, job description, and company details. The goal is to build a model that predicts salary based on the provided features.

## Project Overview
The Salary Prediction project involves multiple steps of a data science and machine learning workflow, including data preprocessing, exploratory data analysis (EDA), model selection, and performance evaluation.

### Key Components:
1. **Importing Necessary Libraries**  
   Libraries such as `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `scikit-learn`, and `plotly` are used for data manipulation, statistical analysis, visualization, and machine learning model development.

2. **Data Preprocessing**  
   - Handle missing values in features like `min_salary`, `max_salary`, and `avg_salary`.
   - Convert categorical features (e.g., `Job Title`, `Company Name`, `Location`) into numerical representations using techniques like label encoding and one-hot encoding.
   - Create new features such as `avg_salary` from `min_salary` and `max_salary`, and extract useful information from textual data (e.g., whether the job requires Python, R, AWS skills).

3. **Exploratory Data Analysis (EDA)**  
   - Visualize relationships between features such as job location, company rating, and salary.
   - Understand the distribution of `Salary Estimate` and identify patterns in job titles, industries, and sectors.
   - Analyze correlations between features like company age, location, and the presence of technologies such as Python, AWS, and Excel.

4. **Model Selection and Training**  
   Multiple machine learning models are implemented to predict salaries, including:
   - **Linear Regression**
   - **Random Forest Regressor**
   - **Gradient Boosting Regressor**

   These models are trained using various evaluation techniques and hyperparameter tuning to optimize performance.

5. **Model Evaluation**  
   - Evaluate models using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score.
   - Compare the performance of different models to select the best-performing one.
   - Visualize model predictions and residuals using `plotly` for enhanced interpretation.

6. **Visualization**  
   Use libraries like `plotly` and `seaborn` to create interactive visualizations for:
   - Salary distribution by job title, location, and industry.
   - Correlation heatmaps to identify the most important features influencing salary predictions.
   - Model performance metrics and error distribution.

## Dataset
The dataset contains the following columns:
- **Job Title**: Title of the job position.
- **Salary Estimate**: Estimated salary range for the job.
- **Job Description**: Detailed description of the job role.
- **Rating**: Company rating.
- **Company Name**: Name of the company offering the job.
- **Location**: Location of the job.
- **Headquarters**: Headquarters of the company.
- **Size**: Company size.
- **Founded**: Year the company was founded.
- **Type of Ownership**: Ownership type of the company (private, public, etc.).
- **Industry**: Industry to which the company belongs.
- **Sector**: Sector of the company.
- **Revenue**: Company's revenue.
- **Competitors**: List of competitors.
- **hourly**: Whether the salary is hourly-based.
- **employer_provided**: Whether the employer provided salary information.
- **min_salary**: Minimum salary.
- **max_salary**: Maximum salary.
- **avg_salary**: Average salary, calculated from `min_salary` and `max_salary`.
- **company_txt**: Processed company name.
- **job_state**: State where the job is located.
- **same_state**: Whether the job is in the same state as the company headquarters.
- **age**: Age of the company.
- **python_yn**: Whether Python is mentioned in the job description.
- **R_yn**: Whether R is mentioned in the job description.
- **spark**: Whether Spark is mentioned in the job description.
- **aws**: Whether AWS is mentioned in the job description.
- **excel**: Whether Excel is mentioned in the job description.
