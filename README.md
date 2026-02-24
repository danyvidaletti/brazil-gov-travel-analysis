# Brazilian Government Travel Expenses Analysis (2025)

## 📌 Project Overview
This project analyses public travel expenses of Brazilian government officials using open data from the **Portal da Transparência** (Brazilian Transparency Portal). The goal of this analysis is to identify travel expenditure patterns, calculate average trip durations, and determine the average costs associated with different public job titles.

## 🛠️ Tools & Technologies
* **Language:** Python
* **Libraries:** Pandas (Data Manipulation), Matplotlib (Data Visualisation)
* **Environment:** Google Colab / Jupyter Notebook

## 🧹 Data Cleaning & Preparation
The dataset contained raw records of individual trips. To prepare the data for analysis, the following steps were taken:
* Handled encoding and localisation issues (`Windows-1252`, European decimal separators).
* Engineered a new `Despesas` (Total Expenses) column by summing up ticket costs, refunds, and other expenses.
* Treated missing values in the `Cargo` (Job Title) column.
* Converted string dates into standard `datetime` formats to calculate the duration of each trip (`Dias de viagem`) and extract the travel month.

## 📊 Data Aggregation & Insights
The data was aggregated by Job Title (`Cargo`) to extract the following metrics:
* Average expense per trip.
* Average trip duration (in days).
* Total expenses per job title.
* Most frequent destinations.
* Total number of trips.

To ensure statistical relevance, the final dataset was filtered to include only job titles representing more than 1% of the total recorded trips. 

## 📈 Visualisations
The analysis concludes with a horizontal bar chart illustrating the **Average Expense per Trip by Job Title**, styled with a custom dark theme for better readability.

## 🚀 How to Run the Project
1. Clone this repository.
2. Ensure you have the dataset downloaded from the *Portal da Transparência* (or use the provided sample if applicable).
3. Update the file paths in the notebook to point to your local directories.
4. Run the Jupyter Notebook to reproduce the tables and charts.
