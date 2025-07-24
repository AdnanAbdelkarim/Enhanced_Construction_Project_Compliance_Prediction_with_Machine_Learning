# 🏗️ Enhanced Construction Projects Compliance Prediction with Machine Learning

This research project explores and improves predictive modeling for construction project compliance using machine learning. It reproduces and enhances results from the original study titled **"Predicting Construction Project Compliance with Machine Learning"**, using the same dataset but refining multiple modeling steps to yield stronger performance.

Conducted under the supervision of **Dr. Uzair Ahmed** at the **University of Doha for Science and Technology**.

---

## 📂 Project Structure

```
Enhanced_Construction_Projects_Compliance/
│
├── dataset/                        # Portuguese Public Procurement dataset (PPPData)
│   └── PPPData_EN_1.0.xlsx
│
├── notebook/                       # Jupyter notebook with full code
│   └── Enhanced_Prediction.ipynb
│
├── paper/                          # Original and enhanced research papers
│   ├── Original_Paper.pdf
│   └── Enhanced_Research_Paper.pdf
│
├── visuals/                        # Block diagram comparison
│   └── block_diagram_comparison.png
│
├── requirements.txt               # Python dependencies
└── README.md                      # Project overview and usage
```

---

## 📊 Dataset

- **Source**: [Portuguese Public Procurement Data (PPPData) – Mendeley](https://data.mendeley.com/datasets/v7smh33bst/1)
- **Description**: Public construction contract records (2015–2022) collected from:
  - 📄 [Portal Base](https://www.base.gov.pt)
  - 📄 Diário da República Eletrónico (DRE)
- **Format**: Excel (.xlsx)
- 📁 Included locally under `dataset/`

---

## 🧠 Methodology Overview

The project aims to classify public construction projects as **compliant** or **non-compliant**, using a Random Forest classifier with key improvements:

- Cleaned and filtered dataset
- Generated target variable based on EPI/IP ratio
- Applied SMOTE to address class imbalance
- Selected relevant features through correlation analysis and permutation importance
- Tuned RandomForest hyperparameters via GridSearchCV

📘 The entire process is implemented in:
```
notebook/Enhanced_Prediction.ipynb
```

📊 Visual workflow comparison is available in:
```
visuals/block_diagram_comparison.png
```

---

## 📈 Results Comparison

| Metric      | Original Paper | This Project (Enhanced) |
|-------------|----------------|--------------------------|
| Accuracy    | 0.832          | **0.89**                 |
| Precision   | 0.830          | **0.88**                 |
| Recall      | 0.866          | **0.89**                 |
| F1-Score    | 0.846          | **0.88**                 |

✅ Enhanced results were achieved through better class balancing and parameter tuning, as detailed in the paper and notebook.

---

## 🛠️ Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/AdnanAbdelkarim/Enhanced_Construction_Project_Compliance_Prediction_with_Machine_Learning.git
   cd Capstone_Projects
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   # On Mac/Linux use: source venv/bin/activate      # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the Jupyter notebook**
   ```bash
   jupyter notebook notebook/Enhanced_Prediction.ipynb
   ```

---

## 📦 Requirements

```
pandas
numpy
scikit-learn
matplotlib
seaborn
imblearn
openpyxl
```

📌 `openpyxl` is required to load `.xlsx` Excel files.

---

## 📄 Papers

- 📘 **Original Paper**: `paper/Original_Paper.pdf`
- 📗 **Enhanced Version**: `paper/Enhanced_Research_Paper.pdf`

---

## 📌 Notes

- All code and visualizations are contained within a single notebook for ease of reproduction.
- Data and visuals are neatly separated into folders.
- Ensure the `dataset/PPPData_EN_1.0.xlsx` file remains in the correct path when running the notebook.

---

## 🙌 Acknowledgements

Supervision: Dr. Uzair Ahmed  
Special thanks to the original study authors for enabling this comparison and enhancement through open data and transparent methodology.

---

## 📜 License & Attribution

Authors: Adnan Abdelkarim and Dr. Uzair Ahmed  
This work is part of an academic research project. Please cite the corresponding publication when referencing this work.

