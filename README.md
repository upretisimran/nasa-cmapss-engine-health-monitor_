# NASA CMAPSS Engine Health Monitor
India Space Academy — AI and ML in Space Exploration

AI-based real-time anomaly detection and autonomous decision support system built on the NASA CMAPSS FD001 turbofan engine degradation dataset.

---

## Project Overview

This project combines unsupervised and supervised machine learning to detect engine anomalies, estimate Remaining Useful Life (RUL), and generate autonomous maintenance decisions in real time.

---

## Models Used

| Model | Type | Purpose |
|---|---|---|
| Isolation Forest | Unsupervised | Anomaly detection |
| Autoencoder | Unsupervised | Reconstruction-error anomaly detection |
| LSTM Classifier | Supervised | Binary degradation classification |
| LSTM RUL Regressor | Supervised | Remaining Useful Life prediction |

---

## Results

| Model | Precision | Recall | F1 | AUC |
|---|---|---|---|---|
| Isolation Forest | 0.756 | 0.913 | 0.827 | 0.875 |
| Autoencoder | 0.216 | 0.216 | 0.216 | 0.640 |
| LSTM Classifier | 0.779 | 0.990 | 0.872 | 0.876 |

RUL Regression: MAE = 11.0 cycles, RMSE = 14.6 cycles

Fleet Health (100 test engines): Critical 25, Warning 16, Normal 59

---

## Repository Structure
```
nasa-cmapss-engine-health-monitor/
├── notebook.ipynb
├── report/
│   ├── technical_report.docx
│   ├── results_confusion_matrix.docx
│   └── future_extension_ideas.docx
├── outputs/
│   ├── plot_model_evaluation.png
│   ├── plot_fleet.png
│   └── realtime_monitor.gif
└── README.md
```

---

## Dataset

NASA CMAPSS FD001 available on Kaggle at https://www.kaggle.com/datasets/bishals098/nasa-turbofan-engine-degradation-simulation

---

## Author

Simran Upreti — India Space Academy, AI and ML in Space Exploration Program
