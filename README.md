# AICTE-Intership-IBMSKill-Project
A machine learning system that detects and classifies power grid faults (like line-to-ground or line-to-line) using electrical data. Built with XGBoost, SHAP, and IBM Cloud, the model achieves 93% accuracy and is ready for real-time deployment.
# Power Fault Detection using Machine Learning

This project is focused on detecting and classifying faults in a power distribution system using machine learning. It aims to identify fault types like **line-to-ground**, **line-to-line**, and **three-phase** using real-time electrical data such as voltage, current, and equipment status. The system is trained on publicly available data and is designed to be accurate, explainable, and ready for deployment.

---

## Project Overview

Power system faults can lead to instability and outages. Early and accurate detection of these faults is critical. This project leverages a **supervised learning pipeline** using **XGBoost**, achieving over **93% classification accuracy**. The model is interpretable using **SHAP values**, and all data is securely accessed through **IBM Cloud Object Storage**.

---

## Key Features

- **ML Algorithms Used**:
- XGBoost (best performance)
- Random Forest
- Support Vector Machine (SVM)

- **Model Accuracy**:

  > **93%** (XGBoost) – evaluated with precision, recall, F1-score, and confusion matrix

- **Deployment Ready**:  
  Trained `.pkl` model included for real-time use in apps or APIs

- **Explainability with SHAP**:  
  Visualizations help interpret how features impact predictions

- **IBM Cloud Integrated**:  
  Data is fetched securely from IBM Cloud Object Storage using `ibm_boto3`

---

## Project Structure

```
power-fault-detection/
├── notebook/                # Jupyter notebook with full pipeline
├── model/                   # Trained XGBoost model (.pkl)
├── data/                    # Source CSV files
├── visuals/                 # Confusion matrix, SHAP plot, etc.
├── report/                  # Final project report (PDF/Word)
├── README.md                # Project documentation (this file)
└── requirements.txt         # List of Python dependencies
```

---

## Dataset

- Source: [Kaggle - Power System Faults Dataset](https://www.kaggle.com/datasets/ziya07/power-systemfaults-dataset)
- Features: Voltage, Current, Component Health, Location
- Labels: Fault Type (Line-to-Ground, Line-to-Line, Three-Phase, etc.)

---

## Technologies Used

- Python (3.8+)
- Scikit-learn
- XGBoost
- SHAP (for model explainability)
- IBM Cloud Object Storage (COS)
- Matplotlib & Seaborn (for visualizations)

---

## Future Enhancements

- Real-time streaming from IoT sensors or SCADA
- Integration with deep learning models like LSTM
- Edge computing deployment (e.g., Raspberry Pi)
- Grid-wide fault visualization dashboards

---

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/power-fault-detection.git
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter notebook:

   ```bash
   jupyter notebook notebook/fault_detection_model.ipynb
   ```

4. Run all cells to train or test the model

---

## Contributors

- **Vignesh Parmar** – Machine Learning Engineer / Author

---

## License

This project is open-source and available under the [MIT License](LICENSE).
