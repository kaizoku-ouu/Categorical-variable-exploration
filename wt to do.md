Here are 30 commands you can try in Python using libraries such as Pandas, Seaborn, and Matplotlib to explore the categorical variables in your dataset.

### 1. Importing Libraries
```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
```

### 2. Loading the Data
```python
df = pd.read_csv('path_to_your_dataset.csv')
```

### 3. Overview of the Data
```python
df.head()
df.info()
df.describe(include='all')
df['Geography'].value_counts()
df['Gender'].value_counts()
df['Card Type'].value_counts()
```

### 4. Bar Plot for Categorical Variables
```python
sns.countplot(x='Geography', data=df)
plt.title('Count of Customers by Geography')
plt.xlabel('Geography')
plt.ylabel('Number of Customers')
plt.show()
```

```python
sns.countplot(x='Gender', data=df)
plt.title('Count of Customers by Gender')
plt.xlabel('Gender')
plt.ylabel('Number of Customers')
plt.show()
```

```python
sns.countplot(x='Card Type', data=df)
plt.title('Count of Customers by Card Type')
plt.xlabel('Card Type')
plt.ylabel('Number of Customers')
plt.show()
```

### 5. Box Plot to Compare Distributions
```python
sns.boxplot(x='Geography', y='CreditScore', data=df)
plt.title('Credit Score Distribution by Geography')
plt.xlabel('Geography')
plt.ylabel('Credit Score')
plt.show()
```

```python
sns.boxplot(x='Gender', y='CreditScore', data=df)
plt.title('Credit Score Distribution by Gender')
plt.xlabel('Gender')
plt.ylabel('Credit Score')
plt.show()
```

```python
sns.boxplot(x='Card Type', y='Balance', data=df)
plt.title('Balance Distribution by Card Type')
plt.xlabel('Card Type')
plt.ylabel('Balance')
plt.show()
```

### 6. Violin Plot for Distribution Comparison
```python
sns.violinplot(x='Geography', y='CreditScore', data=df)
plt.title('Credit Score Distribution by Geography')
plt.xlabel('Geography')
plt.ylabel('Credit Score')
plt.show()
```

```python
sns.violinplot(x='Gender', y='EstimatedSalary', data=df)
plt.title('Estimated Salary Distribution by Gender')
plt.xlabel('Gender')
plt.ylabel('Estimated Salary')
plt.show()
```

```python
sns.violinplot(x='Card Type', y='Point Earned', data=df)
plt.title('Points Earned Distribution by Card Type')
plt.xlabel('Card Type')
plt.ylabel('Points Earned')
plt.show()
```

### 7. Swarm Plot for Detailed Distribution
```python
sns.swarmplot(x='Geography', y='CreditScore', data=df)
plt.title('Credit Score Distribution by Geography')
plt.xlabel('Geography')
plt.ylabel('Credit Score')
plt.show()
```

```python
sns.swarmplot(x='Gender', y='Balance', data=df)
plt.title('Balance Distribution by Gender')
plt.xlabel('Gender')
plt.ylabel('Balance')
plt.show()
```

```python
sns.swarmplot(x='Card Type', y='Satisfaction Score', data=df)
plt.title('Satisfaction Score Distribution by Card Type')
plt.xlabel('Card Type')
plt.ylabel('Satisfaction Score')
plt.show()
```

### 8. Point Plot to Show Mean Values
```python
sns.pointplot(x='Geography', y='CreditScore', data=df)
plt.title('Mean Credit Score by Geography')
plt.xlabel('Geography')
plt.ylabel('Mean Credit Score')
plt.show()
```

```python
sns.pointplot(x='Gender', y='EstimatedSalary', data=df)
plt.title('Mean Estimated Salary by Gender')
plt.xlabel('Gender')
plt.ylabel('Mean Estimated Salary')
plt.show()
```

```python
sns.pointplot(x='Card Type', y='Balance', data=df)
plt.title('Mean Balance by Card Type')
plt.xlabel('Card Type')
plt.ylabel('Mean Balance')
plt.show()
```

### 9. Heatmap for Categorical Variable Relationships
```python
pd.crosstab(df['Geography'], df['Gender'])
sns.heatmap(pd.crosstab(df['Geography', 'Gender']), annot=True, fmt="d")
plt.title('Heatmap of Geography and Gender')
plt.show()
```

```python
pd.crosstab(df['Geography'], df['Card Type'])
sns.heatmap(pd.crosstab(df['Geography', 'Card Type']), annot=True, fmt="d")
plt.title('Heatmap of Geography and Card Type')
plt.show()
```

```python
pd.crosstab(df['Gender'], df['Card Type'])
sns.heatmap(pd.crosstab(df['Gender', 'Card Type']), annot=True, fmt="d")
plt.title('Heatmap of Gender and Card Type')
plt.show()
```

### 10. Pie Chart for Categorical Variables
```python
df['Geography'].value_counts().plot.pie(autopct='%1.1f%%')
plt.title('Proportion of Customers by Geography')
plt.ylabel('')
plt.show()
```

```python
df['Gender'].value_counts().plot.pie(autopct='%1.1f%%')
plt.title('Proportion of Customers by Gender')
plt.ylabel('')
plt.show()
```

```python
df['Card Type'].value_counts().plot.pie(autopct='%1.1f%%')
plt.title('Proportion of Customers by Card Type')
plt.ylabel('')
plt.show()
```

### 11. Pairplot to Explore Relationships
```python
sns.pairplot(df, hue='Geography')
plt.title('Pairplot by Geography')
plt.show()
```

```python
sns.pairplot(df, hue='Gender')
plt.title('Pairplot by Gender')
plt.show()
```

```python
sns.pairplot(df, hue='Card Type')
plt.title('Pairplot by Card Type')
plt.show()
```

### 12. Grouped Statistics
```python
df.groupby('Geography')['CreditScore'].mean()
df.groupby('Gender')['EstimatedSalary'].median()
df.groupby('Card Type')['Balance'].std()
```

### 13. Catplot for Multiple Categorical Plots
```python
sns.catplot(x='Geography', kind='count', data=df)
plt.title('Count of Customers by Geography')
plt.show()
```

```python
sns.catplot(x='Gender', kind='count', data=df)
plt.title('Count of Customers by Gender')
plt.show()
```

```python
sns.catplot(x='Card Type', kind='count', data=df)
plt.title('Count of Customers by Card Type')
plt.show()
```

These commands provide a comprehensive toolkit for exploring categorical variables in your dataset, helping you understand their distributions, relationships, and impacts on other variables.
