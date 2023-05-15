# DS---Customer-Service-Requests-Analysis-Project


The provided code performs various tasks related to data preprocessing, visualization, and statistical analysis using the pandas, numpy, matplotlib, seaborn, statsmodels, and scipy libraries in Python. Here's a breakdown of the code:

1. Importing Required Libraries:
   - pandas: Library for data manipulation and analysis.
   - numpy: Library for mathematical operations.
   - matplotlib.pyplot: Library for data visualization.
   - seaborn: Library for statistical data visualization.
   - statsmodels.api: Library for statistical models and tests.
   - scipy.stats: Library for statistical functions.

2. Reading Data:
   - The code reads the '311_Service_Requests_from_2010_to_Present.csv' file using pandas' `read_csv` function and stores it in the `customers` dataframe.
   - The first few rows of the dataframe are printed using the `head()` function.

3. Exploratory Data Analysis:
   - Descriptive statistics of the dataframe are printed using the `describe()` function.
   - The shape of the dataframe (number of rows and columns) is printed using the `shape` attribute.
   - Visualizations are created to analyze the distribution of complaint types and the number of null values in each column.

4. Data Preprocessing:
   - The records with null values in the 'Closed Date' column are dropped using the `dropna` function.
   - The time elapsed between the closed and creation dates is calculated and stored in a new column.
   - The calculated time elapsed is converted to seconds for better representation.

5. Visualization:
   - Various visualizations are created using matplotlib, seaborn, and pandas to show the distribution of complaints across different cities and visualize the types of complaints.

6. Data Analysis:
   - Statistical analysis is performed to identify significant variables using p-values and a Kruskal-Wallis H test.
   - The average request closing time is visualized, and statistical analysis is performed using the OLS (Ordinary Least Squares) method.
   - The difference in median request closing time between different locations is tested using the Kruskal-Wallis H test.

The code demonstrates the steps involved in data preprocessing, exploratory data analysis, visualization, and statistical analysis of the given dataset. It provides insights into complaint types, cities, and request closing times, and performs statistical tests to analyze significant differences.
