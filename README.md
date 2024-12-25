# Fraud Detection


This dataset can be accessed <a href="https://huggingface.co/datasets/Nooha/cc_fraud_detection_dataset">Here</a>

This project was developed collaboratively with <a href="https://github.com/GulsahKLC">Gülşah Kılıç</a>

<p align="center">
  <img src="https://github.com/user-attachments/assets/668287a2-0f78-42c7-9c4d-920479da14a7" alt="Image description" />
</p>

This project focuses on analyzing a dataset to derive meaningful insights. The analysis involves data preparation, cleaning, and visualization, utilizing Microsoft SQL Server and Tableau. Additionally, sensitive data, such as SSN, was hashed using an irreversible SHA256 algorithm to ensure data privacy.

Tools and Technologies

-	Microsoft SQL Server: Used for data import, cleaning, and analysis.
-	Tableau: Utilized for data visualization and creating impactful dashboards.
-	Advanced Excel: Employed for quick exploratory data analysis and summarization.

1. Data Preparation and Cleaning
   
-	Dataset Import: The dataset was uploaded to Microsoft SQL Server for efficient handling and analysis.
-	Missing and Null Value Analysis: 
-	Identified columns containing null values.
-	Proposed and applied strategies such as imputation or exclusion to handle missing data.
-	Ensured the privacy of sensitive information by hashing the SSN attribute using the SHA256 algorithm, making it irreversible.
-	Data Integration: Combined necessary columns and tables to create a cohesive and usable dataset.
-	SQL Queries: After the datasets were loaded into SQL, they were merged, and each variable was examined individually. Queries were executed using conditional expressions to detect inconsistencies between specific columns. General KPI values were identified using SQL queries.After data retrieval, table merging, and data analysis operations, they were used both in the machine learning process and integrated with Tableau.
-	Imbalanced Dataset Identification: Uneven data distribution was observed and flagged for resolution during the modeling phase.

3. Data Analysis
   
The cleaned dataset was analyzed to extract insights in the following areas:

-	Patterns and Correlations: Identified significant relationships and trends within the data.
-	Outlier Detection: Recognized and flagged anomalous data points for further investigation.
-	Statistical Summaries: Generated descriptive statistics to summarize the dataset.
-	KPI Development: Designed and calculated Key Performance Indicators (KPIs) to support decision-making processes.

4. Data Visualization
   
Data visualization was performed in Tableau to highlight key findings effectively:

-	Interactive Dashboards: Developed user-friendly dashboards for seamless data exploration.
-	Visualization Types: Designed impactful visualizations.
-	Highlighting Trends: Visuals clearly emphasized critical insights and trends.

Example Dashboard Features: 

-	Job Distributions: Showed customer distributions across various job roles.
-	Category Expenditures: Illustrated spending behaviors across different categories.
-	Gender vs. Fraud Analysis: Explored fraud amounts segmented by gender.
-	Geographic Heatmaps: Identified fraud trends and concentrations across different states.
-	Dynamic Filtering: Enabled users to interactively filter and drill down into specific data segments.

(by Gülşah)

<p align="center">
  <img src="https://github.com/user-attachments/assets/cf264b10-ccc7-4cb2-b624-c1a3781a55a3" alt="Image description" />
</p>

# Machine Learning Section
Encoded features were created, and two machine learning models—logistic regression and LightGBM (LGBM)—were developed. The following observations were made based on these models:

# Logistic Regression
Logistic regression was found to be ineffective in classifying the imbalanced dataset. Attempts were made to improve the results by applying cross-validation, resulting in an F1 score of 0.499.

# LGBM
The initial performance of the LGBM model was observed to be worse than that of logistic regression, with an F1 score of 0.12. After applying cross-validation, the F1 score was improved to 0.544.

These outcomes were considered to be the worst results encountered in any project. Consequently, research was conducted, and the Synthetic Minority Oversampling Technique (SMOTE) was applied. After this adjustment, the following metrics were achieved with the LGBM model:

- Accuracy: 0.996
- Precision: 0.299
- Recall: 0.606
- F1: 0.400

# Ensemble Modeling
Further efforts were made to enhance the results, and an ensemble approach was implemented successfully. A deep learning model was integrated with the LGBM model, yielding the best results for the project. The metrics achieved were as follows:

- Accuracy: 0.9983
- Precision: 0.9978
- Recall: 0.9989
- F1: 0.9983
  
(by Mehmet)

<p align="center">
  <img src="https://github.com/user-attachments/assets/7c51445b-f54a-422f-85e1-e83057f94b53" alt="Image description" />
</p>
