# Adult Income Analysis

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3%2B-orange)](https://scikit-learn.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.13%2B-FF6F00)](https://www.tensorflow.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Description
Analysis of the **Adult Income Dataset** from the UCI Machine Learning Repository. The goal is to predict whether an individual's income exceeds **$50,000/year** using various data mining and machine learning techniques.

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
├── src/                                    # Source code
│   ├── part1_data_preprocessing.py         # Data preprocessing (missing values, encoding, normalization, PCA)
│   ├── part2_feature_selection.py          # Feature selection & outlier detection (SelectKBest, Random Forest, Z-score)
│   ├── part3_clustering.py                  # Clustering analysis (K-Means, Hierarchical, Silhouette Score)
│   ├── part4_classification_sklearn.py      # Classification (Logistic Regression, Random Forest)
│   └── part5_neural_network.py              # Neural Network with Keras/TensorFlow (MLP with 2 hidden layers)
│
├── data/                                    # Data (raw & processed)
├── results/                                  # Plots and results
├── report/                                    # Final PDF report
├── requirements.txt                           # Required libraries
└── README.md                                   # Project documentation
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

# 3. Download the dataset
# Download 'adult.data' from UCI repository and place it in the project folder

# 4. Run the analysis stages in order
python src/part1_data_preprocessing.py    # Creates clean_adult_data.csv
python src/part2_feature_selection.py     # Feature selection & outlier detection
python src/part3_clustering.py             # Clustering analysis
python src/part4_classification_sklearn.py # Classification with scikit-learn
python src/part5_neural_network.py         # Neural Network with Keras
```

## 📈 Analysis Stages

### 1️⃣ Data Preprocessing (Part 1)
- Missing value handling (replacement with mode)
- Categorical variable encoding (LabelEncoder)
- Numerical feature normalization (MinMaxScaler)
- Dimensionality reduction with PCA (95% variance)

### 2️⃣ Feature Selection & Outlier Detection (Part 2)
- Correlation analysis with heatmap visualization
- Feature selection using SelectKBest (ANOVA F-value)
- Feature importance with Random Forest
- Performance comparison (all features vs top 5 features)
- Outlier detection using Z-score
- Outlier visualization with boxplots

### 3️⃣ Clustering (Part 3)
- K-Means Clustering (n_clusters=2)
- Hierarchical Clustering (Agglomerative)
- Evaluation with Silhouette Score
- PCA visualization (2D scatter plots)
- Dendrogram visualization

### 4️⃣ Classification with scikit-learn (Part 4)
- Train/test split (80/20)
- Feature normalization with StandardScaler
- Logistic Regression classifier
- Random Forest classifier (n_estimators=100)
- Evaluation: accuracy, precision, recall, F1-score
- Confusion matrices visualization

### 5️⃣ Neural Network with Keras/TensorFlow (Part 5)
- Train/validation/test split (60/10/30)
- Feature normalization with StandardScaler
- MLP architecture:
  - Input layer (64 neurons, ReLU)
  - Dropout layer (0.3)
  - Hidden layer (32 neurons, ReLU)
  - Dropout layer (0.3)
  - Output layer (1 neuron, Sigmoid)
- Training for 30 epochs
- Learning curves visualization (loss & accuracy)
- Confusion matrix evaluation

## 📦 Required Libraries
```
pandas
numpy
scikit-learn
matplotlib
seaborn
tensorflow
keras
scipy
```

## 📝 Results
Results from each stage are saved in the `results/figures/` folder and include:
- `correlation_heatmap.png`
- `feature_importance_rf.png`
- `outliers_boxplots.png`
- Clustering scatter plots
- Confusion matrices
- Neural network training curves

## 📄 Report
The full project report can be found at [`report/adult_income_analysis_report.pdf`](report/adult_income_analysis_report.pdf)

## 📜 License
MIT License - Free use and modification with attribution.

## 📬 Contact
thbazhba@gmail.com
