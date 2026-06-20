# Customer Churn Analysis — Data Science Tools

A complete end-to-end data science project on a customer churn dataset, covering the full pipeline from raw messy data to clustering insights and machine learning classification.

## 📌 Problem Statement

Customer churn (when customers stop using a service) is a major business challenge. This project analyzes a churn dataset to uncover patterns, segment customers, and build predictive models.

## 🗂️ Dataset

**File:** `churn.csv`

The dataset contains customer behavioral and demographic features including login frequency, time spent, wallet points, referral info, and a churn label.

## 🔬 Project Pipeline

### 🧹 Data Cleaning
- Identified and handled dirty values (`?`, `Error`, `Unknown`)
- Fixed impossible negative values in numeric columns
- Replaced errors with median values
- Dropped duplicates and remaining nulls

### 📐 Outlier Removal
- Applied **IQR method** to remove statistical outliers from all numeric columns

### 📊 Exploratory Data Analysis (EDA)
- Column-level inspection: unique values, distributions, descriptive stats
- Visualizations with Matplotlib and Seaborn

### ⚙️ Feature Engineering
- Label encoding for categorical variables
- Standard scaling for numerical features

### 🔻 Dimensionality Reduction
- **PCA** — reduced feature space for visualization and clustering

### 🔵 Clustering Analysis
| Method | Features Used |
|--------|--------------|
| K-Means | RFM features |
| Agglomerative Clustering | RFM features |
| K-Means | Behavioral & Demographic |
| Agglomerative Clustering | Behavioral & Demographic |

- Elbow method and **Silhouette Score** used to find optimal `k`
- Dendrogram visualization for hierarchical clustering

### 🤖 Classification
- Machine learning models from scikit-learn
- Evaluation using accuracy and silhouette scores

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Pandas | Data loading and cleaning |
| NumPy | Numerical operations |
| Matplotlib / Seaborn | Visualization |
| scikit-learn | PCA, clustering, classification, metrics |
| SciPy | Hierarchical clustering and dendrogram |

## 🚀 Getting Started

```bash
# Clone the repository
git clone <repo-url>
cd customer-churn-analysis

# Install dependencies
pip install -r requirements.txt

# Place the dataset
# Make sure churn.csv is in the project root

# Run the notebook
jupyter notebook Customer_Churn_Analysis.ipynb
```

## 👤 Author

**Mohamed Gamal**  
Bachelor of Computer and Information Science — Data Science and AI Department  
Alexandria National University
