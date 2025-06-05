# Implement-the-Sparse-RBM-for-gene-selection-and-classification


A professionally curated machine learning pipeline to classify leukemia subtypes — Acute Myeloid Leukemia (AML) and Acute Lymphoblastic Leukemia (ALL) — using DNA microarray-derived gene expression profiles.

---

## 📌 Project Objective

This project aims to demonstrate a robust and interpretable methodology for classifying leukemia subtypes based on gene expression data. Through rigorous statistical analysis and machine learning modeling, we seek to identify critical gene markers that effectively distinguish AML from ALL, supporting precision medicine and diagnostic research.

---

## 🧬 Dataset Description

* **Source**: Golub et al., 1999 (Science, Vol. 286)
* **Data Type**: Gene expression profiles obtained via DNA microarrays
* **Samples**:

  * 38 training samples
  * 34 independent test samples
* **Features**: 7129 genes per sample, collected from bone marrow and peripheral blood

All expression values have been pre-normalized to ensure chip comparability.

---

## 🧪 Methodological Framework

### 1. **Preprocessing**

* Normalization validation
* Stratified splitting of training and test datasets

### 2. **Feature Selection**

* Applied two-sample **t-tests** across gene features
* Selected top-ranking genes based on statistical significance (p-values)

### 3. **Visualization**

* Generated histograms and KDE plots for the most significant genes
* Analyzed gene expression distributions across AML and ALL groups

### 4. **Classification Modeling**

* Implemented supervised learning algorithms using the selected gene subset
* Performance assessed via metrics such as accuracy, confusion matrix, and ROC-AUC

---

## 🔍 Key Biomarkers

Top three statistically significant genes were further analyzed for their biological functions and relevance to leukemia pathophysiology. These genes demonstrated strong discriminative capacity between AML and ALL samples.

---

## 🛠 Technology Stack

* **Programming**: Python 3
* **Libraries**: NumPy, Pandas, Matplotlib, Seaborn, SciPy, scikit-learn
* **Platform**: Google Colab (Jupyter Notebooks)

---

## 📈 Project Outcomes

* Achieved high classification accuracy using a minimal subset of gene features
* Enhanced interpretability and biological insight through targeted gene analysis
* Provided a foundational framework for future oncology-based expression studies

---

## 📚 Reference

Golub, T. R., Slonim, D. K., Tamayo, P., et al. (1999). Molecular Classification of Cancer: Class Discovery and Class Prediction by Gene Expression Monitoring. *Science*, 286(5439), 531–537.

---

## 🚀 Future Directions

* Expansion to multi-class cancer subtype classification
* Integration with biological pathway and gene ontology databases
* Evaluation using deep learning approaches for large-scale omics data

---

## 📄 License

This repository is intended for academic and research use. Proper citation of the original publication and dataset is required for any reuse or distribution.

---

## 🙏 Acknowledgments

We extend our gratitude to the researchers of the 1999 Golub et al. study for their pioneering work and for making this invaluable dataset publicly accessible.

---

We welcome collaboration and contributions. Please explore, analyze, and enhance the methodology.
