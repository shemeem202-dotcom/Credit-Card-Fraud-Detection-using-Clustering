# Credit Card Fraud Detection using Clustering

## Project Overview
This project focuses on detecting unusual transaction patterns in credit card data using **unsupervised machine learning** techniques.

Since fraud datasets are often highly imbalanced, clustering helps identify suspicious transactions by grouping similar transaction behaviors and isolating anomalies.

---

## Objective
The objective of this project is to detect potential fraudulent transactions using clustering algorithms without relying on labeled fraud data.

Algorithms used:
- **KMeans Clustering**
- **DBSCAN Clustering** *(if used in notebook)*
- **Hierarchical Clustering** *(optional)*

---

## Dataset
Dataset: **Credit Card Fraud Detection Dataset**

Typical features include:
- Time
- Amount
- V1 to V28 (PCA-transformed features)

Target column:
- `Class`
  - 0 = Normal Transaction
  - 1 = Fraud Transaction

For clustering, the target label is usually excluded during training.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

### 1. Import Libraries
Imported libraries for:
- Data analysis
- Visualization
- Clustering
- Preprocessing

### 2. Load Dataset
Loaded the credit card transaction dataset into a Pandas DataFrame.

### 3. Data Preprocessing
Performed:
- Missing value check
- Feature scaling using `StandardScaler`
- Dropping unnecessary columns
- Separating features from target labels

### 4. Exploratory Data Analysis
Analyzed:
- Transaction amount distribution
- Fraud vs non-fraud distribution
- Correlation heatmap

### 5. Clustering Model
Applied clustering algorithms such as:

#### KMeans
- Selected optimal number of clusters
- Assigned cluster labels

#### DBSCAN (if applicable)
- Density-based anomaly detection
- Identified outliers as suspicious transactions

### 6. Visualization
Generated:
- Scatter plots
- Cluster plots
- Fraud anomaly visualization

---

## Results
- Successfully grouped similar transactions
- Detected anomalous/outlier transactions as potential fraud
- Clustering highlighted unusual spending behavior patterns

---

## Key Insights
- Fraudulent transactions often appear as outliers
- Feature scaling is critical for clustering performance
- Unsupervised learning is useful when fraud labels are limited or unavailable

---

## Conclusion
This project demonstrates how clustering techniques can be used for fraud detection in financial transactions.

Using unsupervised learning methods:
- KMeans groups similar transaction behavior
- DBSCAN can identify anomalies effectively
