# Aerofit Treadmill Customer Profiling and Analysis

## Overview

This project aims to analyze customer data for Aerofit Treadmills to understand the customer demographics, usage patterns, and preferences. The analysis includes segmentations based on various factors such as product type, age, gender, education, marital status, usage, fitness level, income, and usage intensity. Additionally, correlation analysis is performed to identify relationships between different features.

## Data

The dataset used for this analysis contains the following features:
- **Product**: Type of treadmill purchased (KP281, KP481, KP781)
- **Age**: Age of the customer
- **Gender**: Gender of the customer
- **Education**: Number of years of education
- **MaritalStatus**: Marital status of the customer (Single, Partnered)
- **Usage**: Average number of times the treadmill is used per week
- **Fitness**: Self-rated fitness level (1 to 5)
- **Income**: Annual income of the customer
- **Miles**: Average number of miles run on the treadmill per week

## Analysis

### 1. Product-based Segmentation
- Count of customers for each product type.

### 2. Age-based Segmentation
- Customers segmented into age groups: Young Adults (18-25), Adults (26-35), Middle-aged (36-50), Seniors (51+).

### 3. Gender-based Segmentation
- Count of customers by gender.

### 4. Education-based Segmentation
- Customers segmented into education groups: High School, Some College, College Graduate.

### 5. Marital Status Segmentation
- Count of customers by marital status.

### 6. Usage-based Segmentation
- Customers segmented into usage groups: Light Users, Moderate Users, Heavy Users.

### 7. Fitness Level Segmentation
- Customers segmented into fitness levels: Beginners, Intermediate, Advanced.

### 8. Income-based Segmentation
- Customers segmented into income groups: Lower Income, Middle Income, Higher Income.

### 9. Usage Intensity Segmentation
- Customers segmented into usage intensity groups: Light Users, Moderate Users, Heavy Users.

### 10. Correlation Analysis
- Correlation heatmap to identify relationships between different features.

## Insights

### Product-based Segmentation
- Determine the most and least popular treadmill models among customers.

### Age-based Segmentation
- Identify the predominant age groups using the products.

### Gender-based Segmentation
- Understand the gender distribution of customers.

### Education-based Segmentation
- Analyze the educational background of customers.

### Marital Status Segmentation
- Assess the impact of marital status on treadmill purchase and usage.

### Usage-based Segmentation
- Classify customers based on their treadmill usage frequency.

### Fitness Level Segmentation
- Understand the fitness levels of customers.

### Income-based Segmentation
- Segment customers based on their annual income.

### Usage Intensity Segmentation
- Identify usage intensity patterns among customers.

### Correlation Analysis
- Explore relationships between features such as age, income, usage, and fitness levels.

## How to Run the Analysis

1. **Load the Dataset**:
   ```python
   import pandas as pd
   df = pd.read_csv('path_to_your_file/aerofit_treadmill.csv')
   ```

2. **Perform Segmentation**:
   Follow the segmentation steps provided in the analysis section to segment customers based on different factors.

3. **Generate Plots**:
   Use the provided plotting functions to visualize the segmentation results.

4. **Correlation Analysis**:
   Calculate and plot the correlation matrix to identify relationships between features.

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Calculate the correlation matrix
correlation_matrix = df.corr()

# Plotting the heatmap
plt.figure(figsize=(12, 8))
sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm', linewidths=0.5)
plt.title('Correlation Heatmap')
plt.show()
```

## Conclusion

This analysis provides valuable insights into customer demographics, usage patterns, and preferences for Aerofit Treadmills. These insights can help in targeted marketing, product development, and enhancing customer satisfaction.

