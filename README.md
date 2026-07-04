# Machine-Learning-Project-M.Tech-
AI &amp; Cybersecurity Researcher focused on intelligent Intrusion Detection Systems. Building hybrid ML/DL security solutions using Random Forest, CNN-BiLSTM, entropy-based adaptive routing, explainable AI (SHAP), and real-time network threat detection.

# Hybrid Intrusion Detection System using Random Forest and CNN-BiLSTM

## Overview

This repository presents a Hybrid Intrusion Detection System (HIDS) that combines a Random Forest classifier with a CNN-BiLSTM deep learning model for accurate network intrusion detection.

The proposed approach utilizes a two-stage architecture:

- **Stage 1:** Random Forest performs fast intrusion detection.
- **Stage 2:** CNN-BiLSTM verifies uncertain predictions to improve detection performance while reducing computational overhead.

The implementation is provided as a single Jupyter Notebook containing the complete workflow from data preprocessing to model evaluation.

---

## Features

- Complete end-to-end implementation
- Data preprocessing and cleaning
- SMOTE-based class imbalance handling
- Feature scaling using MinMaxScaler
- Random Forest classifier
- CNN-BiLSTM deep learning model
- CNN and LSTM baseline models
- Hybrid decision framework
- Cross-validation
- ROC Curve
- Confusion Matrix
- Precision, Recall and F1-score evaluation
- Training accuracy and loss visualization

---

## Repository Structure

```
Hybrid_IDS_Project/
│
├── data/                         # Place datasets here
├── main_complete_v31.ipynb       # Complete implementation
├── calibrated_rf_cicids.pkl
├── calibrated_rf_unsw.pkl
├── random_forest_cicids.pkl
├── random_forest_unsw.pkl
├── deep_model_cicids.keras
├── deep_model_unsw.keras
├── scaler_cicids.pkl
├── scaler_unsw.pkl
├── requirements.txt
└── README.md
```

---

## Datasets

The datasets are **not included** in this repository due to GitHub file size limitations.

This project uses:

### CICIDS2017

Contains modern network traffic including both benign and malicious activities such as:

- DDoS
- DoS
- PortScan
- Botnet
- Brute Force
- Web Attacks
- Infiltration
- Heartbleed

Download:

https://www.unb.ca/cic/datasets/ids-2017.html

---

### UNSW-NB15

Contains normal and malicious network traffic generated using modern attack scenarios.

Download:

https://research.unsw.edu.au/projects/unsw-nb15-dataset

---

## Dataset Placement

After downloading, organize the datasets as follows:

```
data/
│
├── CICIDS/
│      Friday-WorkingHours-Afternoon-DDos.csv
│      ...
│
└── UNSW/
       UNSW_NB15_training-set.csv
       UNSW_NB15_testing-set.csv
```

Update the dataset paths inside the notebook before execution.

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Hybrid_IDS_Project.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
main_complete_v31.ipynb
```

---

## Technologies Used

- Python
- Scikit-learn
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Imbalanced-learn

---

## Results

The notebook includes:

- Data preprocessing
- Model training
- Cross-validation
- Accuracy comparison
- Precision
- Recall
- F1-score
- ROC curves
- Confusion matrices
- Training Accuracy/Loss plots

---

## Citation

If you use this work in your research, please cite the corresponding publication.

---

## License

This project is intended for research and educational purposes.
