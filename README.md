
# Customer Segmentation using KMeans & DBSCAN

This project focuses on **customer segmentation** using the popular **Mall Customers dataset**. The goal is to group customers into meaningful clusters based on their **annual income** and **spending score**.

Customer segmentation helps businesses:

* Identify groups of similar customers
* Target marketing campaigns better
* Improve customer experience

---

## Dataset

* Dataset used: **Mall Customers Dataset** (Kaggle)
* Key features used for clustering:

  * **Annual Income (k\$)**
  * **Spending Score (1-100)**

These two features were chosen because they best represent customer purchasing behavior and financial capacity.

---

##  Steps Followed

### 1. Data Exploration & Visualization

* Loaded the dataset with **Pandas**
* Visualized customer distribution using **Matplotlib**

### 2. Feature Scaling

* Applied **MinMaxScaler** to normalize Annual Income and Spending Score
* Scaling is important because clustering algorithms are distance-based

### 3. Finding Optimal Number of Clusters (KMeans)

* Used the **Elbow Method** by plotting **SSE (Sum of Squared Errors)** against values of k
* Selected the best k where the "elbow" appeared

### 4. KMeans Clustering

* Applied **KMeans** with optimal k
* Visualized the clusters with different colors
* Marked centroids with a star `*`

### 5. Bonus: DBSCAN Clustering

* Tried **DBSCAN** as an alternative clustering algorithm
* Learned how parameters like `eps` and `min_samples` affect clusters
* Compared DBSCAN results with KMeans

### 6. Cluster Analysis

* Analyzed **average spending per cluster**
* Found patterns in how income and spending habits group customers

---

## Results

* KMeans produced **5 distinct clusters** that made business sense
* DBSCAN showed that clustering results are sensitive to parameter tuning
* Each cluster represents a group of customers with similar spending behavior

---

## 🛠️ Tools & Libraries

* Python
* Pandas
* Matplotlib
* Scikit-learn (KMeans, DBSCAN, MinMaxScaler)

---

## Key Learnings

* Importance of feature scaling before clustering
* How to use the **Elbow Method** for choosing k
* Difference between **KMeans (partitioning-based)** and **DBSCAN (density-based)**
* How clustering can help businesses in customer insights

---

## How to Run

1. Clone the repository

   ```bash
   git clone https://github.com/your-username/customer-segmentation.git
   cd customer-segmentation
   ```
2. Install required libraries

   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook or Python script

   ```bash
   jupyter notebook segmentation.ipynb
   ```

---

##  Visualizations

* Scatter plots showing customer groups
* Elbow method plot for selecting k
* DBSCAN clustering results

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

---

✨ This project is part of my **internship tasks**, where I explored clustering algorithms and applied them to real-world datasets.

---
