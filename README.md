# Biomarker Selection from Gene Expression Data Using PCA and RFE

This project explores the identification of gene expression biomarkers for breast cancer classification using a simplified and interpretable approach: **Principal Component Analysis (PCA)**.

It is inspired by the methodology in Al Abir et al. (2022), but diverges by replacing the autoencoder-based feature selection with PCA to assess dimensionality reduction, interpretability, and classification performance under a lighter computational setting.

---

## 🎯 Project Overview

- **Goal:** Identify a minimal set of predictive genes to classify tumor vs. normal tissue in breast cancer.
- **Dataset:** Public mRNA gene expression dataset from GEO (originally used in Al Abir et al., 2022)
- **Techniques:** PCA for feature reduction + Logistic Regression for classification
- **Tools:** Python, pandas, scikit-learn, matplotlib

---

## 🔬 Methodology

- Data preprocessing: cleaning and standardization
- PCA: explored explained variance to determine number of components
- Classification: trained a Logistic Regression model using top PCs
- Evaluation: accuracy, confusion matrix, ROC curve

---

## 📊 Results

- **Top 4–5 principal components** explained ~90% of total variance
- Achieved strong classification performance using reduced features
- PCA allowed interpretable linear projections and visual clustering
- The approach is significantly simpler and more explainable than autoencoder-based methods

---

## ⚖️ Comparison to Al Abir et al. (2022)

| Aspect                  | Al Abir et al. (2022)                  | This Project (Alternative Approach)       |
|------------------------|----------------------------------------|-------------------------------------------|
| Dimensionality Reduction | Autoencoder (deep learning)            | PCA (linear projection)                   |
| Feature Selection       | Recursive Feature Elimination (RFE)    | Top PCA components                        |
| Model Complexity        | Neural network-based                   | Logistic Regression                       |
| Interpretability        | Low                                    | High                                      |
| Computational Cost      | High                                   | Low                                       |

---

## 📚 Reference

Al Abir, T., Murtuza, S., Rahman, M., & Rahman, M. S. (2022).  
*Biomarker identification by reversing the learning mechanism of an autoencoder and recursive feature elimination.*  
Computational and Structural Biotechnology Journal, 20, 1840–1850.  
[https://doi.org/10.1016/j.csbj.2022.01.044](https://doi.org/10.1016/j.csbj.2022.01.044)

---

## 🚫 Dataset Disclaimer

The dataset used is based on public gene expression data but is **not included** in this repository due to copyright and data distribution limitations.  
Please refer to the original article or access public repositories like [GEO](https://www.ncbi.nlm.nih.gov/geo/) to request the dataset.

---

## 👩🏻‍💻 About Me

Carmen Sandate  
Post-Degree Diploma in Data Analytics – Langara College  
💼 [Portfolio](https://sandate.vercel.app) | 🧠 [LinkedIn](https://www.linkedin.com/in/mariacarmensandate/)

---
