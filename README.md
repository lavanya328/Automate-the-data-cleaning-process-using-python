Project Requirements: python 3,pandas,numpy,openpyxl,xlrd,os library,program tested(pycharm)
Step-by-Step Process
1. Input and File Verification
The application begins by asking the user for the dataset path and dataset name.
It verifies if the path is valid and checks whether the file is in a supported format (CSV or Excel).
2. Duplicate Detection and Removal
The application checks for duplicate records in the dataset.
Duplicate records are saved as a separate file named {dataset_name}_duplicates.csv.
Duplicate rows are then removed from the main dataset.
3. Handling Missing Values
The application checks for missing values in the dataset.
For numeric columns (integer or float), missing values are replaced by the column’s mean.
For non-numeric columns, rows containing missing values are dropped.
4. Exporting Clean Data
Once cleaned, the dataset is saved as {dataset_name}_Clean_data.csv, and a message confirming successful cleaning is displayed.
5. Multiple Testing & Performance Tuning
The application has been tested with more than 5 different datasets, each containing over 10,000 rows. It consistently cleaned datasets in a matter of seconds, without errors.
The program was also tested using Jupyter Notebook, where it performed flawlessly, allowing easy integration with data science workflows.
Key Features
Fast & Efficient: Cleans large datasets (10k+ rows) in seconds.
Duplicate Backup: Keeps a backup of all duplicate records before removing them.
Missing Values Handling: Automatically fills missing numeric values and drops rows with missing non-numeric values.
User-friendly Prompts: Guides the user step by step with appropriate messages and delay prompts.
Multiple Formats Supported: Handles CSV and Excel files seamlessly.
