# Prog_Multi_Model_Stacking

Implementation of a **multi-model stacking ensemble** for **Bitcoin transaction classification** using the Elliptic Bitcoin Dataset.

The repository accompanies the research on ensemble learning for detecting illicit Bitcoin transactions and provides a complete implementation of the proposed stacking framework, including data preprocessing, model training, hyperparameter optimization, statistical evaluation, and visualization.

---

## Overview

This project implements a stacking ensemble consisting of four optimized base classifiers and a Logistic Regression meta-model.

The workflow includes:

- Data preprocessing
- Feature engineering
- Hyperparameter optimization
- Out-of-fold prediction generation
- Meta-model training
- Performance evaluation
- Statistical comparison of classifiers
- ROC curve visualization
- Precision–Recall curve visualization

---

## Implemented Models

### Base Learners

- Random Forest
- XGBoost
- LightGBM
- CatBoost

### Meta-Learner

- Logistic Regression

---

## Evaluation Metrics

The models are evaluated using the following performance measures:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Precision–Recall AUC (PR-AUC)

Additional statistical comparison is performed using:

- McNemar Test

---

## Experimental Workflow

The notebook contains the complete experimental pipeline:

1. Load and preprocess the Elliptic Bitcoin Dataset
2. Prepare training and testing subsets
3. Train Random Forest
4. Train XGBoost
5. Train LightGBM
6. Train CatBoost
7. Generate Out-of-Fold predictions
8. Train the Logistic Regression meta-model
9. Produce stacking predictions
10. Evaluate all classifiers
11. Compare model performance
12. Perform McNemar statistical tests
13. Plot ROC curves
14. Plot Precision–Recall curves

---

## Repository Structure

```
Prog_Multi_Model_Stacking/
│
├── Prog_Multi_Model_Stacking.ipynb      # Main Jupyter Notebook
├── requirements.txt                     # Python dependencies
├── README.md
├── LICENSE
└── data/
```

---

## Dataset

This project uses the **Elliptic Bitcoin Dataset**.

The dataset is **not included** in this repository.

Download it from:

https://www.kaggle.com/datasets/ellipticco/elliptic-data-set

Create the directory

```
data/
```

and place the following files inside:

```
elliptic_txs_classes.csv
elliptic_txs_features.csv
elliptic_txs_edgelist.csv
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/oterentiev/Prog_Multi_Model_Stacking.git
```

Move to the project directory

```bash
cd Prog_Multi_Model_Stacking
```

Install all required packages

```bash
pip install -r requirements.txt
```

Launch the notebook

```bash
jupyter notebook
```

Open

```
Prog_Multi_Model_Stacking.ipynb
```

---

## Software Requirements

The experiments were performed using

| Package | Version |
|----------|---------|
| Python | 3.11.4 |
| NumPy | 1.26.2 |
| pandas | 2.1.4 |
| scikit-learn | 1.3.2 |
| XGBoost | 3.2.0 |
| LightGBM | 4.5.0 |
| CatBoost | 1.2.10 |
| matplotlib | 3.8.2 |
| statsmodels | 0.14.1 |

---

## Results

The repository reproduces all experiments presented in the accompanying publication, including:

- Comparative evaluation of individual classifiers
- Stacking ensemble evaluation
- Confusion matrices
- Classification reports
- ROC curves
- Precision–Recall curves
- McNemar statistical significance tests

---

## Reproducibility

All experiments are fully reproducible using the provided notebook, the specified software versions, and the publicly available Elliptic Bitcoin Dataset.

---

## Citation

If you use this software in your research, please cite the accompanying publication.

A Zenodo DOI will be added after the first public release.

---

## License

This project is distributed under the **MIT License**.

---

## Author

**Oleksandr Terentiev**

Institute of Telecommunications and Global Information Space  
National Academy of Sciences of Ukraine

GitHub:

https://github.com/oterentiev
