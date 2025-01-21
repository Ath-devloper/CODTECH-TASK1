# DATA PIPELINE DEVELOPMENT  
**COMPANY:** COTECH IT SOLUTIONS

**NAME:** Atharv Phadtare 

**INTERN ID:** CT6WLFX 

**DOMAIN:** DATA SCIENCE

**BATCH DURATION:** JAN 9TH, 2025 to FEB 25th, 2025  

**MENTOR NAME:** NEELA SANTHOSH  

**DESCRIPTION OF TASK**
ETL Task Description

The ETL (Extract, Transform, Load) process is a fundamental component of any data pipeline, where raw data is prepared for analysis or further processing. The ETL task we executed involved designing and implementing a robust pipeline that performed several critical operations, culminating in a clean and structured dataset ready for machine learning or business insights.

Objective
The objective of the ETL task was to extract data from a raw CSV file, perform necessary transformations such as cleaning, encoding, and splitting, and then load the processed data into separate output files for further downstream tasks. This process ensures data consistency, removes redundancies, and standardizes the format, making it more suitable for advanced analytics or predictive modeling.

Steps Involved
Extract Phase
The extraction phase involved reading a raw CSV file located in a specified directory. The file contained diverse columns, some of which were irrelevant or had missing data. The dataset was loaded into memory using Python's Pandas library, which is well-suited for handling structured data.
Input File Path:
The file used for extraction was located at C:\Users\HP\Desktop\6th sem\data.csv.csv. The dataset was analyzed for its structure, including columns, data types, and the presence of missing values.
Transform Phase
Data Cleaning:
The first step in transformation involved removing irrelevant columns such as Series_title_4 and Series_title_5, which were not necessary for our analysis. The errors parameter was set to "ignore" to ensure the script executed even if the columns were missing in the dataset.

Handling Missing Values:
Missing values were dropped using the dropna() method. This ensured that the data used in subsequent processes was complete and reliable.

Encoding Categorical Data:
Categorical columns were identified and encoded into numeric formats using Pandas' LabelEncoder. This step converted textual information into numerical values, which are essential for compatibility with machine learning algorithms.

Feature Selection and Target Identification:
The dataset was split into features (X) and the target variable (y). The target column was specified as target_column, which represents the dependent variable for prediction. All other columns were considered independent features.

Data Splitting:
Using the train_test_split function from Scikit-learn, the data was divided into training and testing sets in an 80:20 ratio. This split is a standard practice to ensure that the model can be validated on unseen data.

Load Phase
The processed data was saved into separate CSV files for training and testing purposes:
train_data.csv for training features.
test_data.csv for testing features.
train_labels.csv and test_labels.csv for corresponding target labels.
Output Directory:
The files were stored in the specified output folder located at C:\Users\HP\Desktop\6th sem\output. Pandas' to_csv method was used to ensure the data was stored efficiently and could be retrieved without loss of formatting.
Challenges Faced
During the ETL process, a few challenges were encountered:

File Path Issues: Initially, incorrect file paths resulted in FileNotFoundError. This was resolved by carefully verifying and using raw string literals (r'...') to handle Windows file paths.
Output Directory Errors: An OSError occurred due to invalid characters or issues in the directory path. The solution involved double-checking the folder path and ensuring it was accessible.
Tools and Libraries Used
Pandas: For data manipulation and transformation.
Scikit-learn: For data splitting and preprocessing.
Python (3.13): As the core programming language for the pipeline.
Outcome
The ETL pipeline successfully transformed the raw data into a clean, structured format. The training and testing datasets were saved in the desired output directory, ready for use in machine learning workflows. This task showcased the importance of ETL in data preprocessing, as it ensured the data was error-free, consistent, and suitable for analytical tasks.

This hands-on ETL task not only improved our understanding of handling data pipelines but also demonstrated the critical role of transformation in preparing data for further processing. By automating the ETL steps, we laid the groundwork for scalability and efficiency in data-driven projects.

#INPUT


#OUTPUT
[test_data.csv](https://github.com/user-attachments/files/18485222/test_data.csv)
[test_labels.csv](https://github.com/user-attachments/files/18485223/test_labels.csv)
[train_data.csv](https://github.com/user-attachments/files/18485220/train_data.csv)
[train_labels.csv](https://github.com/user-attachments/files/18485221/train_labels.csv)
