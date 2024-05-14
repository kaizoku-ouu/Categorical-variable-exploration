# What is a Categorical Variable
- **Definition:** A categorical variable (also known as a qualitative variable) is one that has two or more categories but there is no intrinsic ordering to the categories.\
 **Examples:** Gender (Male, Female), Blood Type (A, B, AB, O).\
[more on categorical data in pandas](https://pandas.pydata.org/docs/dev/user_guide/categorical.html)
# What is a Continuous Variable
- **Definition:** A continuous variable is one that can take any value within a range. These values are often measured and can be infinitely precise.\
**Examples:** Height, Weight, Temperature.

# what is a Discrete Variable
- **Definition:** A discrete variable is one that can take only specific values (often integers) and are countable.\
**Examples:** Number of children in a family, Number of cars in a parking lot.

# Why do we need Categorization Variable Exploration

Exploring variables is a crucial first step in data analysis and machine learning. It involves examining your data closely to understand its characteristics and relationships, helping you make better decisions later on.

Categorization variable exploration is essential for several reasons:

- Data Understanding: Helps in understanding the distribution and frequency of categories.
- Data Cleaning: It helps in Data Cleaning, identifies inconsistencies, missing values, and errors in categorical data.
- Feature Engineering: Helps in transforming and encoding categorical variables for machine learning models.
- Insight Extraction: Provides valuable insights about the relationships between categorical variables and target outcomes.

# Topics to Cover in Categorization Variable Exploration.

 let's dive into how to effectively do this exploration to achieve our analytical goals.
 
-  Identifying Category Variables:
      - Look for variables that represent qualitative characteristics or attributes, such as Geography, Gender, or Card Type, rather than numerical values.
-  Frequency Distribution
      - Analyze how often each category occurs in the dataset, helping to identify dominant categories and rare occurrences.
      -  **Example:** The frequency distribution of Geography shows that there are 5,000 customers from France, 2,500 from Spain, and 2,500 from Germany.( using value_counts() )
-  Missing Values
      - Check for any missing values in categorical variables, which may require imputation or special handling to maintain data integrity.
      - **Example:** In the dataset, some customers may have missing values for the Balance variable
-  Encoding Categorical Variables
      - Convert categorical variables into numerical representations suitable for machine learning algorithms, such as one-hot encoding or label encoding.
      - **Example:** Suppose we have a categorical variable Gender with values 'Male' and 'Female'. Using label encoding, 'Male' can be encoded as 0 and 'Female' as 1. 
-  Grouping and Aggregation
      - Group categorical variables to analyze data at a higher level of abstraction, aggregating information for meaningful insights, such as calculating average income by Geography.
      - **Example:** Grouping the data by Geography and calculating the mean CreditScore for each country provides insights into average credit scores across different regions.
-  Visualizing Categorical Data :
    - **Bar Plot:** The bar plot shows the number of customers from each geography, providing a quick visual comparison of the customer distribution.
    - **Box Plot:** The box plot displays the spread and central tendency of credit scores for customers in each geography, revealing any differences or similarities in 
         credit scores among different regions.
    - **Histogram:** A histogram is useful for visualizing the distribution of a single continuous variable. For example, we can create a histogram for the CreditScore variable to see its distribution.

