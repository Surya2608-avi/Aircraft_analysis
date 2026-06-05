# Aircraft_analysis
The Aircraft Analysis notebook implements a structured machine learning pipeline to evaluate aircraft safety using sensor data. The main goal is to predict risk levels based on operational parameters such as vibration (RMS), temperature, RPM, and acoustic noise, which are key indicators of aircraft performance and potential faults.
The workflow begins with data loading and exploratory data analysis (EDA). Basic operations like viewing dataset structure, summary statistics, and correlations help in understanding the distribution and relationships between features. This step ensures clarity about data patterns before modeling.

Next, data preprocessing is carried out to improve data quality. Missing values are handled using mean and median imputation techniques, and duplicate records are removed. This ensures the dataset is clean and reliable for further analysis.

The notebook also uses the Polars library for efficient data transformation. Filtering conditions are applied to identify extreme values such as high temperature, vibration, RPM, and noise, which may indicate risky situations. Aggregation functions are used to summarize data based on risk categories.

An important feature of the project is data validation using Great Expectations. Validation rules check for null values, acceptable ranges, and data consistency, ensuring the dataset meets quality standards and supports Responsible AI practices.

Finally, a logistic regression model is built to predict risk. The data is split into training and testing sets, and feature scaling is applied using StandardScaler. Model performance is evaluated using accuracy and confusion matrix.

Overall, the project demonstrates an end-to-end approach to aircraft risk prediction using data preprocessing, validation, and machine learning techniques.
