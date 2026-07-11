# Task 4: Unsupervised Learning (PCA + K-Means Clustering) 🛍️

Applying **Unsupervised Learning** techniques — K-Means Clustering for customer segmentation and Principal Component Analysis (PCA) for dimensionality reduction.

## 📋 Project Overview

This project segments mall customers into distinct groups based on their **Age**, **Annual Income**, **Spending Score**, and **Gender**, using K-Means Clustering. PCA is then used to reduce dimensionality and visualize the clusters in 2D.

## 📊 Dataset

- **Source**: [Kaggle - Mall Customer Segmentation Data](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)
- **File used**: `Mall_Customers.csv` (included in this repo — 200 rows, 5 columns)
- **Features**: CustomerID, Gender, Age, Annual Income (k$), Spending Score (1-100)

## 🛠️ Tech Stack

- Python 3.10+
- Scikit-Learn (KMeans, PCA, StandardScaler)
- Pandas / NumPy
- Matplotlib / Seaborn
- Jupyter Notebook

## 📁 Project Structure

```
├── Task4_Unsupervised_Learning_PCA_KMeans.ipynb   # Main notebook
├── requirements.txt                                # Python dependencies
├── .gitignore
└── README.md
```

## 🚀 How to Run

1. Clone this repository
```bash
git clone <your-repo-url>
cd <your-repo-name>
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook
```bash
jupyter notebook
```

4. Open `Task4_Unsupervised_Learning_PCA_KMeans.ipynb` and run all cells (dataset is already included)

## 📈 Workflow

1. **Data Loading & Exploration** — Inspect structure, check for missing values
2. **EDA** — Gender distribution, feature distributions, income vs spending score, correlation heatmap
3. **Preprocessing** — Label encode Gender, scale features with `StandardScaler`
4. **Optimal K Selection** — Elbow Method + Silhouette Score
5. **K-Means Clustering** — Segment customers into groups
6. **Cluster Visualization** — Income vs Spending Score scatter plot by cluster
7. **PCA** — Reduce to 2 components, visualize clusters in PCA space, check explained variance
8. **Cluster Profiling** — Understand what each segment represents (avg age, income, spending)
9. **Validation** — Predict cluster for new hypothetical customers
10. **Export** — Save segmented dataset as `customer_segments.csv`

## ✅ Outcome

- Clear customer segments identified for targeted marketing
- Dimensionality reduction applied and visualized using PCA
- Reusable clustering pipeline for similar customer datasets

## 📝 Author

Your Name Here

## 📄 License

This project is open source and available under the MIT License.
