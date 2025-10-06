# 🛍️ Customer Segmentation Using Unsupervised Learning (LRFS + Autoencoder + K-Means)

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)](https://www.tensorflow.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-yellow?logo=scikitlearn)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-App-red?logo=streamlit)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

##  Overview

This project focuses on customer segmentation using unsupervised learning techniques to understand and categorize online shopping behaviors.  
By applying the LRFS (Length, Recency, Frequency, Staying rate) model, Autoencoder-based dimensionality reduction, and K-Means clustering, we identify key customer groups based on behavioral patterns.  

This segmentation helps e-commerce platforms:
- Personalize marketing strategies  
- Improve customer retention  
- Increase conversion rates  

---

##  Project Workflow

| Phase | Description |
|:------|:-------------|
| Phase 0 | Environment setup and library installation |
| Phase 1 | Exploratory Data Analysis (EDA): Trend visualization, purchase behavior study |
| Phase 2| LRFS Feature Engineering: Extracted Length, Recency, Frequency, Staying rate |
| Phase 3 | Dimensionality Reduction using Autoencoder and t-SNE |
| Phase 4 | Clustering & Profiling using K-Means and K-Medoids |
| Phase 5 | Explainability, Visualization (Plotly), and Streamlit Dashboard creation |

---

## 🧠 Methodology

### 🧾 Step 1: Data Understanding
- Dataset: Online Shoppers Intention Dataset (UCI / Kaggle)
- Shape: ~12,000 rows × 18 features  
- Key columns: *Administrative, Informational, ProductRelated, Month, SpecialDay, Revenue*

### ⚙️ Step 2: LRFS Feature Engineering
Derived new behavioral features:
| Feature | Description |
|----------|--------------|
| **L (Length)** | Total number of session visits |
| **R (Recency)** | Time since last visit |
| **F (Frequency)** | Number of visits over a period |
| **S (Staying Rate)** | Average duration of interaction |

### 🧩 Step 3: Autoencoder Dimensionality Reduction
- Reduced LRFS feature space to **2 latent dimensions** (`Dim1`, `Dim2`)
- Captures hidden relationships in user behavior data.

### 🔮 Step 4: K-Means Clustering
- Applied K-Means (k=4) for segmentation
- Evaluated cluster quality using **Silhouette Score**
- Visualized cluster distribution in latent space.

### 🧭 Step 5: Explainability & Visualization
-  model interpretation.  
- Created interactive charts using **Plotly** and **Seaborn**.  

---

##  Results

| Cluster | Segment Name | Conversion Rate | Key Behavior |
|:--------:|:-------------|:----------------|:--------------|
| 0 | 🟡 Occasional Shoppers | 25% | Moderate frequency and recent visits |
| 1 | 🔵 New Explorers | 24% | New users exploring the site |
| 2 | 🔴 Window Shoppers | 8% | Low engagement, quick exits |
| 3 | 🟢 Loyal Frequent Buyers | 41% | High frequency, strong loyalty |

### 🧩 Business Insights
- **Cluster 3** customers are most valuable; should be rewarded with loyalty benefits.  
- **Cluster 2** users show low engagement; target with reactivation campaigns.  
- **Clusters 0 & 1** can be converted with personalized offers.

---

##  Tech Stack

| Category | Technologies |
|-----------|---------------|
| **Language** | Python 3.10 |
| **Data Handling** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn, Plotly |
| **Machine Learning** | Scikit-learn, TensorFlow, K-Means, Autoencoder |
| **Deployment** | GitHub / Streamlit Cloud |

---




