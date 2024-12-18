# Final-Report
# The last report of the course

## Project Overview
This project aims to analyze the trends of AI adoption in the job market by exploring anonymized data on job roles, salaries, industries, and AI adoption levels. The findings will provide valuable insights for businesses, policymakers, and job seekers to make informed decisions.

## Dataset Information
Source: AI-Powered Job Market Insights Platform
Data Type: Tabular Data
Domain: Job Market Analysis
Feature Types: Mixed (Categorical and Numerical)
Missing Values: None
## Attribute Information
The dataset includes the following columns:

Job_Title: The title of the job role
Industry: The industry of the job
Company_Size: The size of the company
Location: Job location
AI_Adoption_Level: The level of AI adoption in the company
Automation_Risk: The risk of automation for the role
Required_Skills: Skills required for the job
Salary_USD: Annual salary in USD
Remote_Friendly: Whether the job supports remote work
Job_Growth_Projection: Projected growth for the role

## Project Background
What is the AI-Powered Job Market Study?
Artificial Intelligence (AI) significantly influences the future of the job market. Key aspects include:

Leading Industries in AI Adoption: Understanding which industries are at the forefront of AI implementation.
Salary Trends Analysis: Examining salary trends across different roles, industries, and risk levels.
Relationship Between AI Adoption and Remote Work Opportunities: Evaluating how AI adoption correlates with the availability of remote work.
This study provides valuable insights to help businesses, policymakers, and job seekers make informed decisions.

## Why Choose AI for This Analysis?
AI enables data-driven insights, including:

Predicting Future Job Roles and Salary Trends: Forecasting how job roles and salaries will evolve.
Assessing Automation Risks for Specific Roles: Evaluating which roles are at higher risk of automation.
Analyzing Correlations Between Job Growth Projections and Salaries: Understanding how projected job growth relates to salary changes.
By leveraging machine learning and visualization tools, we aim to extract actionable insights for strategic planning.

## Directory Structure
├── data
│   └── ai_job_market_insights.csv
├── models
│   ├── job_market_trends.ipynb
│   └── ai_job_predictions.json
├── presentation
│   └── Job_Market_Analysis.pptx

## Data Preparation and Visualization
### Tools Used
Programming Language: Python
Libraries: Pandas, Numpy, Matplotlib, Seaborn

###  Data Cleaning and Processing
Removing Duplicates: Eliminated duplicate rows from the dataset.
Data Type Conversion: Converted categorical variables to appropriate data types.
Creating Salary Range: Categorized salaries into Low, Medium, and High based on distribution.

### Visualization Analysis
Salary Distribution: Visualized the overall distribution of salaries.
AI Adoption Level Distribution: Displayed the frequency of different AI adoption levels.
Boxplot of Salary by AI Adoption Level: Analyzed salary distribution across AI adoption levels.
Boxplot of Salary by Remote Work Friendly: Examined salary variations for remote-friendly positions.
Average Salary by Top 10 Industries: Showed average salaries across the top ten industries.
Average Salary by Automation Risk: Analyzed the relationship between automation risk and salary.
Heatmap of AI Adoption Level by Company Size: Illustrated AI adoption levels across different company sizes.

## Modeling and Classification

## Objectives
Industry Classification: Predict the industry type (Manufacturing, Technology, Education) based on salary levels and automation risk.
Modeling Techniques:
Logistic Regression: Suitable for binary and multi-class classification.
Random Forest Classifier: Robust and flexible for industry prediction.

## Data Preparation
Feature Engineering: Created salary ranges and filtered the top three industries by frequency. Applied dummy encoding for salary ranges.
Data Splitting: Divided data into 80% training and 20% testing sets. Applied standard scaling to numerical features.

## Model Evaluation

### Logistic Regression
Description: A statistical model that in its basic form uses a logistic function to model a binary dependent variable. It is suitable for both binary and multi-class classification tasks.

Best Hyperparameter:
C: 1.0 (Regularization strength)
Accuracy: 37%

Confusion Matrix Insights:
The confusion matrix indicates balanced predictions with slight misclassifications between the Technology and Manufacturing industries.

### Random Forest Classifier
Description: An ensemble learning method that operates by constructing multiple decision trees during training and outputting the mode of the classes for classification tasks. It is known for its robustness and flexibility.

Best Hyperparameters:
Number of Estimators (n_estimators): 200
Maximum Depth (max_depth): 10
Accuracy: 37%

Confusion Matrix Insights:
Similar to Logistic Regression, the Random Forest Classifier also shows an accuracy of 37%, with comparable misclassification patterns between Technology and Manufacturing industries.

## Process Summary
This project successfully analyzed AI adoption trends in the job market and classified industries based on salary ranges. Key findings include:

Leading Industries: Manufacturing, Technology, and Education are at the forefront of AI adoption.
Salary and Automation Risk Correlation: High automation risk is associated with lower salaries, particularly in roles involving repetitive tasks.
Model Performance: The Random Forest Classifier provided the most accurate predictions for industry classification.

## Key Findings and Recommendations
Industry Leadership: Manufacturing, Technology, and Education industries lead in AI adoption. Businesses should monitor AI developments in these sectors.
Salary and Risk Correlation: Positions with high automation risk tend to have lower salaries. Policymakers and educational institutions should focus on upskilling and reskilling in these areas.
Remote Work Opportunities: There is a noticeable correlation between AI adoption and remote work opportunities. Companies can leverage this trend to optimize their human resource strategies.
## Future Work
Add More Features: Incorporate additional features such as required skills and job location to enhance prediction accuracy.
Advanced Models: Utilize more sophisticated models like Gradient Boosting and Neural Networks for salary prediction.
In-depth Analysis: Further investigate the long-term impact of AI adoption on various job roles and industries.
