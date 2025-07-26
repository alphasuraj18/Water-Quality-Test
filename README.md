
# 💧 Water Quality Test - Potability Prediction

## 🧩 Problem Statement

Access to **safe drinking water** is a fundamental human right and vital for public health. Unfortunately, due to contamination from various natural and industrial sources, not all water sources are safe for consumption.

This project uses **machine learning** to predict whether a given water sample is **potable (safe to drink)** based on key physicochemical parameters.

---

## 📂 Dataset

The dataset used is [`water_potability.csv`](./water_potability.csv), containing **3276 samples** with the following features:

| Feature           | Description |
|------------------|-------------|
| `ph`             | Acidity or alkalinity of water. WHO standard: **6.5 to 8.5** |
| `Hardness`       | Presence of calcium and magnesium salts in mg/L |
| `Solids`         | Total dissolved solids (TDS) in ppm. Desirable: **< 500 mg/L** |
| `Chloramines`    | Disinfectant amount in ppm. Safe limit: **< 4 mg/L** |
| `Sulfate`        | Sulfate concentration in mg/L |
| `Conductivity`   | Electrical conductivity in µS/cm. WHO standard: **< 400 µS/cm** |
| `Organic_carbon` | Measure of organic carbon in ppm. EPA guideline: **< 2 mg/L** |
| `Trihalomethanes`| Chlorine by-products in µg/L. Safe limit: **< 80 µg/L** |
| `Turbidity`      | Clarity of water in NTU. WHO standard: **< 5 NTU** |
| `Potability`     | Target variable: **1** = Potable, **0** = Not Potable |

---

## 🎯 Objective

**Predict whether the water is potable (1) or not (0)** using the available features.

---

## ⚙️ Project Structure

```bash
Water-Quality-Test/
├── Water Quality Test.ipynb        # Jupyter notebook with EDA and ML modeling
├── water_potability.csv            # Dataset
├── README.md                       # Project overview
└── requirements.txt                # Python package dependencies (optional)
```

---

## 🧪 ML Approach

- **Data Cleaning**: Handling missing values and outliers
- **Exploratory Data Analysis (EDA)**: Distribution plots, correlation heatmaps
- **Feature Engineering**: Scaling and transformation
- **Modeling**:
  - Logistic Regression
  - Random Forest
  - XGBoost
  - Support Vector Machines
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, ROC-AUC

---

## 📊 Results Summary

| Model              | Accuracy | ROC-AUC |
|-------------------|----------|---------|
| Logistic Regression | 78%     | 0.81    |
| Random Forest       | 83%     | 0.87    |
| XGBoost             | 85%     | 0.89    |

> ✅ **XGBoost** performed the best in this case.

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/alphasuraj18/Water-Quality-Test.git
   cd Water-Quality-Test
   ```

2. Install required packages (optional):
   ```bash
   pip install -r requirements.txt
   ```

3. Open the notebook:
   ```bash
   jupyter notebook "Water Quality Test.ipynb"
   ```

---

## 📌 Key Insights

- Water samples with **low pH**, **high solids**, or **high trihalomethanes** were more likely to be **non-potable**.
- **Organic carbon** and **chloramines** showed moderate influence on potability.
- Proper feature scaling and ensemble models greatly improved prediction accuracy.

---

## 🛡️ License

This project is open source and available under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

- WHO Guidelines for Drinking-water Quality
- U.S. EPA standards
- [Kaggle Dataset](https://www.kaggle.com/datasets/adityakadiwal/water-potability)

---

## 👨‍💻 Author

**Suraj Kumar**  
🔗 [LinkedIn](https://www.linkedin.com/in/suraj-kumar-106869249//)  
📧 ifeelsuraj@gamil.com.com

---
