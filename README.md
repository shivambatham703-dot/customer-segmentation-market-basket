# Customer Segmentation and Market Basket Analysis

Hands-on Lab Evaluation 4 (Module IV) for Data Analytics using Python (CSL0312).
Submitted by Shivam Batham.

## What this repo is about

A retail company wants to know two things:

1. What kinds of customers does it have? (clustering on the Mall Customers data)
2. Which products do people tend to buy together? (association rules on the Groceries data)

This repo holds the datasets and the code I used to answer both.

## Folder structure

```
.
├── data/
│   ├── Mall_Customers.csv
│   └── Groceries_dataset.csv
├── notebook/
│   └── clustering_and_association.ipynb
├── src/
│   └── clustering_and_association.py
├── outputs/
│   └── (cluster graphs and screenshots)
└── README.md
```

## Datasets

| File | Rows | Source |
|------|------|--------|
| Mall_Customers.csv | 200 | Kaggle: vjchoudhary7/customer-segmentation-tutorial-in-python |
| Groceries_dataset.csv | 38,765 | Kaggle: heeraldedhia/groceries-dataset |

## Algorithms used

- K-Means with the Elbow Method
- Hierarchical (Agglomerative) clustering with a dendrogram
- DBSCAN
- Apriori and FP-Growth (via mlxtend), compared on support, confidence, lift and run time

## How to run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn scipy mlxtend
python src/clustering_and_association.py
```

The notebook can also be opened directly in Jupyter or Google Colab.
