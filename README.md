# 🍽️ Zomato Customer Segmentation & Exploratory Data Analysis (EDA)

## 📁 Project Overview
This project involves an end-to-end data analysis pipeline using datasets from Zomato's operations:
- **Orders**
- **Customers**
- **Restaurants**

The goal is to:
- Explore patterns across food orders, locations, cuisines, and customer behavior.
- Perform customer segmentation using **K-Means clustering**.
- Visualize insights and interpret key trends.

---

## 📊 Data Sources
1. **Orders.csv**  
   Contains transactional data such as order IDs, delivery times, payment methods, total amount, and associated customer and restaurant IDs.

2. **Customers.csv**  
   Includes customer details like location, age group, rating, and name.

3. **Restaurants.csv**  
   Provides restaurant-specific information including name, location, cuisine type, cost, ratings, reviews, and operational hours.

---

## 🧪 Steps Performed

### 1. 📥 Data Loading & Cleaning
- Loaded all three datasets using `pandas`.
- Checked for nulls, duplicates, data types.
- Added new columns like `Month`, `Weekday`, `Hour`, and `Delay`.

### 2. 📈 Exploratory Data Analysis (EDA)
- Most ordered dishes and top cuisines.
- Time-based order trends.
- Payment method distributions.
- Customer behavior by location and age.
- Restaurant popularity and review distributions.
- Delivery delays and order status breakdown.

### 3. 🤖 Machine Learning – K-Means Clustering
- Merged all datasets into a unified DataFrame.
- Scaled numeric columns using `StandardScaler`.
- Applied K-Means clustering (`n_clusters=5`).
- Used PCA for 2D visualization of clusters.
- Each cluster represents a unique customer segment.

---

## 📌 Key Insights

- **5 Customer Segments** identified based on order behavior, ratings, and payment patterns.
- **Cluster 0** represents high-value or loyal customers.
- **Cluster 4** contains spread-out customers, likely inconsistent or one-time users.
- **Popular Dishes** like Paneer Tikka, Egg Fried Rice, and Garlic Naan span across multiple cities.
- **American and Indian cuisines** top the popularity charts.
- Most **orders happen in the evening**, with UPI and Cash as dominant payment modes.

---

## 📎 Libraries Used
- `pandas` — Data loading & manipulation
- `seaborn`, `matplotlib` — Visualization
- `numpy` — Numerical analysis
- `scikit-learn` — Clustering and PCA

