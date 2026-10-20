# KMeans-Customer-Segmentation-Project
# 🛍️ Mall Customer Segmentation using K-Means

Customer segmentation project that groups mall customers into distinct segments based on their annual income and spending score using the K-Means clustering algorithm.

<img width="452" height="429" alt="image" src="https://github.com/user-attachments/assets/c69b2d2c-c472-4ec9-bc05-042d367eeb57" />


## 📌 Project Overview

Understanding customer groups helps businesses target marketing, tailor offers, and improve retention. This project applies unsupervised learning to find natural customer segments in the Mall Customers dataset.

## 📊 Dataset

- **Size:** 200 customers, 5 columns

| Column | Description |
|---|---|
| CustomerID | Unique customer ID (dropped in analysis) |
| Gender | Male / Female |
| Age | Customer age |
| Annual Income (k$) | Yearly income in thousands of dollars |
| Spending Score (1-100) | Score assigned by the mall based on spending behavior |

## 🔍 Methodology

1. **Data inspection:** checked for missing values (none found) and summary statistics.
2. **Exploratory Data Analysis (EDA):** distributions of gender, age, income, and score, plus scatter plots between features.
3. **Feature selection:** chose Income and Spending Score, the pair that showed clear groupings.
4. **Scaling:** applied `StandardScaler`.
5. **Clustering:** trained K-Means with `k-means++` initialization.
6. **Choosing K:** used the Elbow Method (inertia for k = 2 to 10).
7. **Visualization:** plotted the final clusters.

## 👥 Customer Segments

The EDA and the Elbow Method both point to **5 clusters**:

1. Low Income, Low Spending
2. High Income, Low Spending
3. Mid Income, Mid Spending
4. Low Income, High Spending
5. High Income, High Spending

<img width="539" height="351" alt="image" src="https://github.com/user-attachments/assets/fb29894f-62d9-43b1-b660-c0ef83847e8c" />

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## 📁 Repository Structure

```
├── clustering-k-means.ipynb
├── Mall_Customers.csv
├── requirements.txt
├── images/
└── README.md
```



