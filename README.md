🩺 Breast Cancer Classification using Neural Network

Classifying breast tumors as Benign or Malignant with a TensorFlow/Keras Artificial Neural Network:-
---
📖 Table of Contents:
- [Overview](#-overview)
- [Dataset](#-dataset)
- [Methodology](#️-methodology)
- [Model Architecture](#-model-architecture)
- [Results](#-results)
- [Repository Structure](#-repository-structure)
- [Tech Stack](#-tech-stack)
- [How to Run](#-how-to-run)
- [Future Scope](#-future-scope)
- [Author](#-author)

---

📌 Overview:
Early and accurate diagnosis is one of the strongest predictors of successful breast cancer treatment. This project builds a compact **Artificial Neural Network (ANN)** that learns to classify tumors as **benign** or **malignant** from digitized cell-nuclei measurements, and packages it into a simple predictive system.

The full workflow — data loading, preprocessing, model design, training, evaluation, and prediction — was carried out as part of the **AI Domain Internship** at **Naviotech Solution Pvt. Ltd.**

📊 Dataset:
| Detail | Value |
|---|---|
| **Source** | Breast Cancer Wisconsin (Diagnostic) Dataset — via `sklearn.datasets` |
| **Samples** | 569 |
| **Features** | 30 numeric features (mean, error, worst of cell-nuclei measurements) |
| **Target** | `0` → Malignant · `1` → Benign |
| **Missing values** | None |

🛠️ Methodology:
1. Loaded the dataset and converted it into a pandas DataFrame
2. Explored the data — shape, summary statistics, class distribution
3. Separated features (`X`) and target (`Y`)
4. Split into training (80%) and testing (20%) sets
5. Standardized features using `StandardScaler`
6. Built and trained a feed-forward Neural Network with TensorFlow/Keras
7. Evaluated performance on unseen test data
8. Visualized training accuracy/loss curves
9. Built a reusable predictive system for new patient samples

🧠 Model Architecture:

Input Layer     → Flatten (30 features)
Hidden Layer    → Dense(20, activation='relu')
Output Layer    → Dense(2, activation='sigmoid')

Optimizer : Adam
Loss      : Sparse Categorical Crossentropy
Epochs    : 10


📈 Results:
| Metric | Score |
|---|---:|
| **Test Accuracy** | **94.74%** |
| **Test Loss** | **0.1289** |

The model generalizes well, with validation accuracy tracking closely with training accuracy across epochs and no signs of overfitting.

 📁 Repository Structure:

├── Breast_Cancer_Classification.py                          # Python script
├── Breast_Cancer_Classification_with_Neural_Network.ipynb    # Jupyter Notebook
├── Cancer_Classification_Report.docx                         # Project report
└── Cancer_Classification.pptx                                # Presentation

 🧰 Tech Stack:
`Python` · `TensorFlow` · `Keras` · `NumPy` · `Pandas` · `Matplotlib` · `scikit-learn`

 ▶️ How to Run:

# Clone the repository
git clone <repo-url>
cd <repo-folder>

# Install dependencies
pip install tensorflow scikit-learn pandas numpy matplotlib

# Run the script
python Breast_Cancer_Classification.py

# OR open the notebook
jupyter notebook Breast_Cancer_Classification_with_Neural_Network.ipynb


🚀 Future Scope:
- Hyperparameter tuning to further improve accuracy
- Benchmark ANN against SVM, Random Forest, and other ML algorithms
- Deploy as a web application for real-time predictions
- Validate on larger, more diverse breast cancer datasets

👤 Author:
**Deepali Das**
B.Tech CSE (Data Science), Gandhi Engineering College, Bhubaneswar
AI Domain Intern, Naviotech Solution Pvt. Ltd. — June 2026 Batch

---
⭐ If you found this project useful, consider giving it a star!
