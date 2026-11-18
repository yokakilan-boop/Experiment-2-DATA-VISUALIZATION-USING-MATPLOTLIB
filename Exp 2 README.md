# Experiment 2: Data Visualization Using Matplotlib and Seaborn

## Aim

To visualize data using Matplotlib and Seaborn libraries.

## Algorithm

1.  **Start.**
2.  Import the Matplotlib and Seaborn libraries.
3.  Load data into a Pandas DataFrame.
4.  Plot a histogram for age distribution using `plt.hist()`.
5.  Plot a scatter plot for Age vs. Salary using `sns.scatterplot()`.
6.  Plot salary distribution using `sns.boxplot()`.
7.  Show the plots sequentially.
8.  **Stop.**


## Program


# Step 1: Import libraries
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Step 2: Create a dataset
data = {
    'Age': [22, 25, 28, 30, 32, 35, 38, 40, 45, 50],
    'Salary': [20000, 25000, 30000, 35000, 40000,
               45000, 50000, 55000, 60000, 65000]
}

df = pd.DataFrame(data)

print("Dataset:")
print(df)

# Step 3: Plot Histogram for Age Distribution
plt.figure(figsize=(6, 4))
plt.hist(df['Age'], bins=5, color='skyblue', edgecolor='black')
plt.title("Age Distribution")
plt.xlabel("Age")
plt.ylabel("Frequency")
plt.show()

# Step 4: Scatter Plot for Age vs Salary
plt.figure(figsize=(6, 4))
sns.scatterplot(x='Age', y='Salary', data=df)
plt.title("Age vs Salary")
plt.xlabel("Age")
plt.ylabel("Salary")
plt.show()

# Step 5: Box Plot for Salary Distribution
plt.figure(figsize=(6, 4))
sns.boxplot(y='Salary', data=df)
plt.title("Salary Distribution")
plt.ylabel("Salary")
plt.show()



## output

1. Histogram – Age Distribution
<img width="562" height="455" alt="image" src="https://github.com/user-attachments/assets/d9c4c3a3-e2d0-463d-990e-c59b107187e4" />

2. Scatter Plot – Age vs Salary

<img width="597" height="357" alt="image" src="https://github.com/user-attachments/assets/7dc2ecdf-0aa6-4b77-af51-349cc139410e" />

3. Box Plot – Salary Distribution
<img width="1310" height="786" alt="image" src="https://github.com/user-attachments/assets/10be5f45-0f0f-4a94-8e50-e195e79f20bc" />


## result
Thus, data visualization was successfully performed using Matplotlib and Seaborn libraries. Histogram, scatter plot, and box plot were created to understand age and salary distributions.

