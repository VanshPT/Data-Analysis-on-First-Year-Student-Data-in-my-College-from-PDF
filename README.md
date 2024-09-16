# Student Admission Data Analysis

## Overview

This project focuses on analyzing the data of students admitted into our college. The raw data was extracted from a PDF document using **Natural Language Processing (NLP)** techniques and libraries like **NLTK** and **Regular Expressions** (RE). After extracting the relevant information, we performed extensive **data cleaning, feature engineering**, and **data analysis**, revealing insightful trends and patterns within the dataset.

## Steps Involved

### 1. Data Extraction (NLP)
- **PDF Parsing**: The student admission data was embedded in a PDF document. We used Python libraries to read and parse the text data.
- **Text Processing with NLP**: Using **NLTK** and **Regular Expressions (RE)**, we processed the extracted text. Key attributes like `meritno`, `gender`, `category`, and `marks` were captured to construct a usable dataset for analysis.

### 2. Data Cleaning
- **Handling Duplicates**: We checked for and removed duplicate entries in the dataset to ensure data integrity.
- **Missing Data**: Missing values were identified and handled appropriately to prevent skewed analyses.
  
### 3. Feature Engineering
- **Category Encoding**: Categories such as **OPEN**, **OBC**, **SEBC**, and **SC** were cleaned and standardized. Additionally, we separated specific subcategories (e.g., **PH**, **DEF**) to enable deeper insights into the data.
- **Gender Encoding**: Male (1) and Female (0) were encoded to streamline gender-based analyses.

### 4. Data Visualization and Exploratory Data Analysis (EDA)
We employed various visualization techniques to uncover key insights:

- **Correlation Heatmap**: We analyzed the correlation between different numerical variables, such as marks and merit numbers.
- **Admission Numbers by Category and Gender**: Using histograms and bar charts, we visualized the distribution of admissions across different categories and genders.
- **Marks and Rank Distribution**: Scatter plots and box plots were used to explore how marks and ranks were distributed across categories and gender.
- **Outlier Analysis**: We identified and analyzed outliers in the marks and merit number data.

### 5. Hypothesis Testing
We formulated and tested the following hypotheses:

- **Hypothesis 1: Admission Performance by Category**
  - **Null Hypothesis (H₀)**: There is no significant difference in the average marks between different admission categories (OPEN, OBC, SEBC, SC).
  - **Alternative Hypothesis (H₁)**: There is a significant difference in the average marks between different admission categories.

Using an **ANOVA test**, we analyzed the significance of the difference in average marks between categories.

## Key Insights
- **Admission Trends**: Certain categories like **OPEN** had higher admission numbers compared to others.
- **Gender Analysis**: The gender ratio varied significantly across categories, with some categories having a higher percentage of males than females.
- **Marks Distribution**: We found notable differences in the performance of students from different categories, and these were backed by our hypothesis tests.

## Tools and Libraries Used
- **Python**: The primary programming language for the project.
- **NLP Tools**: 
  - **NLTK**: For processing and extracting data from the PDF.
  - **Regular Expressions (RE)**: For text cleaning and pattern matching during data extraction.
- **Data Analysis**: 
  - **Pandas**: For data manipulation and cleaning.
  - **Matplotlib & Seaborn**: For visualizing data trends and correlations.
  - **SciPy & Statsmodels**: For performing hypothesis tests like ANOVA.

## Conclusion and Next Steps
This analysis uncovered valuable insights into admission patterns and student performance. Moving forward, further data could help us understand:
1. Admission trends over time if historical data is available.
2. More granular analysis based on student backgrounds or previous educational institutions.
3. Further significance testing on additional hypotheses.

**Request for Additional Data**: 
- To enhance the scope of this analysis, obtaining more detailed data on **student demographics**, **previous academic performance**, and **admission dates** could offer deeper insights into trends over time and across various groups.

