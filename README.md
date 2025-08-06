Association Rule Mining with Apriori and FP-Growth
Submitted by: Banoj Kumar Jena
MSCS 634 – Data Mining
Lab 6 Assignment
Project Overview
This project demonstrates the use of Association Rule Mining techniques to uncover meaningful patterns from transactional data. Using the Online Retail Dataset, we apply both the Apriori and FP-Growth algorithms to identify frequent itemsets and generate association rules. The primary goal is to analyze purchasing behavior and extract insights that could be useful in marketing strategies, inventory planning, and recommendation systems.

Objectives
Preprocess and clean the Online Retail dataset

Transform the data into a suitable format for association mining

Apply the Apriori algorithm to identify frequent itemsets

Apply the FP-Growth algorithm for comparison

Generate association rules based on support, confidence, and lift

Visualize the frequent patterns and interpret business insights

Dataset
The dataset used in this project is an Excel file named Online Retail.xlsx. It contains transactional data for a UK-based online retail company. The data includes the following key fields:

Invoice Number

Stock Code

Description of Item

Quantity

Invoice Date

Unit Price

Customer ID

Country

Only transactions from the United Kingdom are used for this analysis.

Methodology
Step 1: Data Preparation
Removed rows with missing values and negative quantities

Filtered transactions only from the United Kingdom

Transformed the dataset into a basket format suitable for association mining

Step 2: Exploratory Data Analysis
Plotted the top 10 most frequently purchased items using a bar chart

Gained insights into customer purchase preferences

Step 3: Frequent Itemset Mining
Used the Apriori algorithm to identify itemsets with at least 2 percent support

Repeated the same process using FP-Growth to compare speed and output

Visualized the top 10 frequent itemsets from each method

Step 4: Association Rule Generation
Derived association rules from Apriori itemsets using confidence and lift thresholds

Created a scatter plot to visualize rule strength

Key Findings
Popular items such as "WHITE HANGING HEART T-LIGHT HOLDER" often appeared in frequent itemsets

FP-Growth was computationally more efficient compared to Apriori

Rules with lift greater than 2 indicated strong positive associations between item pairs

Challenges
The original dataset required extensive cleaning due to missing and duplicate records

Apriori algorithm was computationally intensive on larger subsets

Memory management was critical for handling high-cardinality itemsets

Technologies Used
Python

Pandas

Matplotlib and Seaborn for visualization

Mlxtend for Apriori, FP-Growth, and association rules

How to Run
Install the required libraries:

pandas

matplotlib

seaborn

mlxtend

Place the dataset Online Retail.xlsx in the project directory

Run the script in a Python environment such as Jupyter Notebook or VS Code

View visualizations and printed outputs for frequent itemsets and association rules

Conclusion
This lab showcases how data mining techniques like association rule mining can provide actionable insights into customer purchasing patterns. The Apriori and FP-Growth algorithms each have their strengths, and using both can help validate findings and improve recommendation systems.
