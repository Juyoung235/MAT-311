# Credit Card Fraud Exploratory Data Analysis

## Project Overview

This MAT311 assignment explores relationships between credit card
transaction characteristics and fraud. The dataset, card_transdata.csv,
was downloaded from the course materials on Brightspace.

The notebook includes data inspection, missing value handling,
distribution plots, within-group fraud comparisons, and scatter plots.
The original dataset contains 999 transactions and eight columns.
After removing 22 rows with missing values, 977 transactions remain.
This project covers exploratory data analysis only.

## AI Assistance

I used OpenAI ChatGPT — GPT-6.1 Sol Medium to help organize the analysis,
generate Python code with comments, explain calculations, and discuss
the results. I ran the code locally in a VS Code Jupyter notebook and
reviewed the outputs during the conversation. The original conversation was conducted
in Korean, and English translations were used for documentation.

## How to Run

Keep the notebook and card_transdata.csv in the same folder.
Open the notebook in VS Code with Jupyter support, select a Python
environment with pandas, matplotlib, seaborn, and ipykernel installed,
and run all cells in order.

## Reflection on AI Assistance

AI helped me work more efficiently by organizing the assignment into clear steps and generating code with comments. Setting expectations early, such as working step by step and including explanations, made it easier to work with the AI without repeating the same instructions. The comparison of chip usage and online orders with fraud was especially helpful. Looking only at transaction counts could be confusing because the groups had different sizes. Showing counts and percentages together made the differences easier to interpret.

However, using AI without understanding data science could lead to incorrect conclusions. For example, someone might confuse a higher number of fraudulent transactions with a higher fraud rate, or assume that PIN usage prevents all fraud because no fraudulent PIN transactions appeared in this sample. During the analysis, we checked that removing 22 incomplete rows reduced the dataset from 999 to 977 transactions. We also reviewed the percentage calculation to confirm that it used each group's total rather than the entire dataset. For example, the fraud rate for transactions without a chip was 63 divided by 673, or about 9.36%. These checks mattered because code can run successfully while still answering the wrong question.