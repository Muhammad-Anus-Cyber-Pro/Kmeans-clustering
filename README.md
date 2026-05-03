# 🧠 Customer Segmentation using K-Means Clustering

## 📌 Overview
This project applies **Unsupervised Machine Learning (K-Means Clustering)** to segment mall customers based on their **annual income** and **spending score**.  
The goal is to identify distinct customer groups to help in better marketing and business decision-making.

---

## 📊 Dataset
- Source: Mall Customers Dataset (public dataset)
- Features used:
  - Annual Income (k$)
  - Spending Score (1–100)

---

## ⚙️ Project Workflow

### 1. Data Loading & Exploration
- Loaded dataset using Pandas
- Checked shape, missing values, and summary statistics

### 2. Feature Selection
- Selected relevant features:
  - Annual Income (k$)
  - Spending Score (1–100)

### 3. Data Preprocessing
- Applied **StandardScaler** to normalize features

### 4. Finding Optimal Clusters
- Used **Elbow Method**
- Plotted WCSS vs number of clusters
- Selected **K = 5**

### 5. Model Training
- Applied **KMeans Clustering**
- Trained model with optimal clusters
- Assigned cluster labels to customers

### 6. Visualization
- Plotted clusters using scatter plot
- Visualized customer segmentation based on income and spending behavior

### 7. Model Evaluation
- Evaluated clustering using **Silhouette Score**

---

## 📈 Results
- Successfully segmented customers into **5 distinct groups**
- Clusters show meaningful differences in spending behavior and income levels

---

## 🛠️ Technologies Used
- Python 🐍
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📌 Key Learnings
- Understanding of **Unsupervised Learning**
- Importance of **feature scaling** in clustering
- How to use **Elbow Method** for optimal K selection
- Cluster evaluation using **Silhouette Score**
- Real-world application of customer segmentation

---

## 📊 Visual Output
(Add your cluster plot image here)

```python
plt.scatter(df['Annual Income (k$)'],
            df['Spending Score (1-100)'],
            c=df['Clusters'])
plt.title("Customer Segmentation")
plt.show()

👨‍💻 Author

Muhammad Anas
AI Engineer | Machine Learning Enthusiast