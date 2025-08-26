

# Longitudinal Mental Health Analysis Dashboard

A comprehensive data science project analyzing how early-life emotional support influences adult mental health outcomes, using the [Add Health dataset](https://www.icpsr.umich.edu/web/ICPSR/studies/21600/variables).

---

## 🚀 Features

- **Modern Workflow**: Reproducible research with Jupyter Notebooks  
- **Data Cleaning & Processing**: Variable selection, encoding, and preprocessing  
- **Statistical Analysis**: Correlation, regression, and hypothesis testing  
- **Machine Learning Models**: Random Forest Regression, SVM Classifier  
- **Visualizations**: Matplotlib & Seaborn for clear, publication-quality charts  
- **Interpretability**: Focus on actionable insights and accessible communication  

---

## ⚡ Quick Start

### Local Development

Clone the repository:

```bash
git clone https://github.com/alyssaqle/COGS-108---Longitudinal-Mental-Health-Analysis.git
cd COGS-108---Longitudinal-Mental-Health-Analysis
```

Open the notebooks in Jupyter or VS Code:

```bash
jupyter notebook
# or use VS Code's built-in notebook support
```

---

## 📂 File Structure

COGS-108---Longitudinal-Mental-Health-Analysis/  
├── FinalProject_Group055_SP25.ipynb    # Main analysis notebook  
├── DataCheckpoint_Group055_SP25.ipynb  # Data cleaning and preparation  
├── EDACheckpoint_Group055_SP25.ipynb   # Exploratory data analysis  
├── ProjectProposal_Group055_SP25.ipynb # Project proposal and planning  
└── README.md  

---

## 📊 Data Sources

This project uses the National Longitudinal Study of Adolescent to Adult Health (Add Health) public-use dataset, including:

- Early-life factors: breastfeeding duration, parental care, involvement in hobbies  
- Adult outcomes: mental health diagnoses, depressive symptoms, counseling usage  
- Waves 1 and 4: adolescence → adulthood progression  

---

## 📈 Results

- **Random Forest Regressor**: Modest predictive power, with best R² = 0.13 for expected education level (edu_exp_a)
- **SVM Classifiers**: Achieved 62–80% accuracy, recall up to 57% for identifying at-risk individuals (depression, arrest history, suicide ideation)
- Findings show stronger predictive links between parental care and adult well-being than for purely clinical outcomes

---

## 🛠️ Technologies

- Python (Pandas, NumPy) for data processing  
- Jupyter Notebooks for analysis and documentation  
- Matplotlib, Seaborn for visualization  
- scikit-learn for machine learning  

---

## 👥 Authors

- Alexandro Merida Silva  
- Adam Rolander  
- Alyssa Le  
- Enrique Aranda  
- Hikari Gregersen  

---

## 📜 License

For academic use only. Dataset subject to Add Health terms of use.
