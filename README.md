# Adult Income Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3%2B-orange)](https://scikit-learn.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Description
Analysis of the **Adult Income Dataset** from the UCI Machine Learning Repository. The goal is to predict whether an individual's income exceeds **$50,000/year** using data mining and machine learning techniques.

This project was implemented as part of the **"Statistical Methods for Data Mining"** course and includes 5 stages of analysis.

## 📊 Dataset
- **Source:** [UCI ML Repository - Adult Dataset](http://archive.ics.uci.edu/ml/datasets/Adult)
- **Records:** 48,842
- **Features:** 14 (demographic & occupational attributes)
- **Target:** Income (>50K or ≤50K)

## 🗂️ Project Structure
```
adult-income-analysis/
│
├── src/                          # Source code
│   ├── part1_data_preprocessing.py  # Data preprocessing
│   ├── part2_feature_selection.py   # Feature selection
│   ├── part3_clustering.py          # Clustering
│   ├── part4_classification_sklearn.py # Classification with scikit-learn
│   └── part5_neural_network.py      # Neural network with Keras/TensorFlow
│
├── data/                         # Data (raw & processed)
├── results/                       # Plots and results
├── report/                         # Final PDF report
├── requirements.txt                # Required libraries
└── README.md                       # Project documentation
```

## 🚀 Installation & Execution

### Prerequisites
- Python 3.8+
- pip (package installer)

### Execution Steps
```bash
# 1. Clone the repository
git clone https://github.com/ThodBaz7/adult-income-analysis.git
cd adult-income-analysis

# 2. Install libraries
pip install -r requirements.txt

# 3. Run the analysis stages
python src/part1_data_preprocessing.py
python src/part2_feature_selection.py
python src/part3_clustering.py
python src/part4_classification_sklearn.py
python src/part5_neural_network.py
```

## 📈 Analysis Stages

### 1️⃣ Data Preprocessing (Part 1)
- Missing value handling (replacement with mode)
- Categorical variable encoding (LabelEncoder)
- Numerical feature normalization (MinMaxScaler)
- Dimensionality reduction with PCA (95% variance)

### 2️⃣ Feature Selection & Outlier Detection (Part 2)
- Correlation analysis (correlation heatmap)
- Feature importance with Random Forest
- Outlier detection using IQR

### 3️⃣ Clustering (Part 3)
- K-Means Clustering
- DBSCAN
- Comparison with ground truth (income)

### 4️⃣ Classification with scikit-learn (Part 4)
- Train/test split (80/20)
- Random Forest Classifier
- Evaluation: accuracy, precision, recall, F1-score

### 5️⃣ Neural Network with Keras/TensorFlow (Part 5)
- Train/validation/test split (60/10/30)
- MLP with 2 hidden layers
- Experimentation with neuron counts

## 📦 Required Libraries
```
pandas
numpy
scikit-learn
matplotlib
seaborn
tensorflow
keras
```

## 📝 Results
Results from each stage are saved in the `results/figures/` folder and summarized in the PDF report.

## 📄 Report
The full project report can be found at [`report/adult_income_analysis_report.pdf`](report/adult_income_analysis_report.pdf)

## 📬 Contact
thbazhba@gmail.com
