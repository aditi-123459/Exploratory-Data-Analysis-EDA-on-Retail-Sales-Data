# Customer Data Exploration & Feature Engineering

## 📌 Project Overview
This project explores a customer dataset to understand demographic patterns, tenure, and distributions.  
It includes data cleaning, feature engineering, exploratory data analysis (EDA), and visualizations to extract insights.  
The goal is to prepare the dataset for downstream tasks like classification or regression and provide clear analysis results.  

The derived features like **Age** and **CustomerTenure_Years** are important numeric variables for understanding customer behavior and preparing for predictive modeling.

## Dataset Description
The dataset contains customer demographic attributes including dates, categories, and other features.

### Key Columns Used / Derived:
- **BirthDate** – Customer’s date of birth  
- **JoinDate** – Customer’s joining date  
- **Gender** – Categorical gender label  
- **City** – Customer’s city  
- **Age** – Derived numeric feature from BirthDate  
- **CustomerTenure_Years** – Derived numeric feature from JoinDate  
- **JoinYear** – Year of JoinDate

### Total Records:
200

### Total Features:
7

## Technologies Used
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Google Colab  

## Project Workflow

1. **Importing Required Libraries**  
2. **Loading Dataset**  
3. **Initial Data Exploration**  
   - Displaying columns (`df.columns`)  
   - Checking info (`df.info()`)  
   - Checking shape (`df.shape`)  
4. **Checking Missing Values**  
   - `df.isnull().sum()`  
5. **Handling Missing Values**  
   - Forward fill / appropriate imputation  
6. **Removing Duplicates**  
   - `df.drop_duplicates(inplace=True)`  
7. **Date Conversion**  
   - Converting `BirthDate` and `JoinDate` to datetime  
8. **Feature Engineering**  
   - Deriving `Age` from `BirthDate`  
   - Deriving `CustomerTenure_Years` from `JoinDate`  
9. **Exploratory Data Analysis (EDA)**  
   - Summary statistics (`df.describe()`)  
   - Distribution counts (`value_counts()`)  
10. **EDA Visualizations**  
    - Gender bar chart  
    - Age histogram  
    - Top 10 cities bar chart  
    - Join year trend line chart  
11. **Correlation Analysis**  
    - Heatmap for numeric features

## EDA & Visualizations

### Distribution & Category Insights
- Gender distribution showed the balance of male vs female customers  
- Age histogram revealed customer age spread across the dataset  
- Top 10 cities showed where most customers are located  
- Join year trend displays how customer registrations changed over time

###  Correlation Analysis
Correlation heatmap between numeric variables helped identify relationships and potential feature interactions.

##  Key Insights

- Customer ages and tenure vary widely, indicating diverse customer profiles  
- Certain cities dominate the dataset in terms of customer count  
- Features like **Age** and **CustomerTenure_Years** are useful numeric attributes for modeling  
- EDA helps uncover patterns before model building

## Conclusion

This project demonstrates a structured **data exploration and feature engineering workflow**.  
Data was cleaned, transformed, explored, and visualized to reveal meaningful patterns and prepare it for predictive modeling tasks.

### Future Improvements
- Feature encoding for modeling  
- Outlier analysis & handling  
- Adding additional meaningful features  
- Building predictive models (e.g., classification or regression)

## Author
Aditi
