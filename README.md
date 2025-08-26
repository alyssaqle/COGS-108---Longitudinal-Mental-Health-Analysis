


# Longitudinal Mental Health Analysis 🧠
---

## ⭐ For a detailed explanation of the project, including the methodology and results, please refer to the [Final Project Notebook](Notebooks/FinalProject_Group055_SP25.ipynb).

---

## 📝 Summary

What separates adults with strong mental health from those who struggle? 

That’s the question we set out to answer by analyzing longitudinal survey data from over 1,700 individuals in the Add Health study, tracking their journey from adolescence to adulthood.

Using statistical analysis and machine learning, we found that higher early-life emotional support—measured by parental care, breastfeeding duration, and involvement in hobbies—was strongly associated with better adult mental health outcomes.

To capture both complex relationships and the ability to flag at-risk individuals, we used two main models:
- **Random Forest Regression** was chosen for its ability to model nonlinear relationships and rank feature importance, providing modest predictive power for adult education level (best R² = 0.13).
- **Support Vector Machine (SVM) Classifiers** were selected for their robustness in high-dimensional, imbalanced data and their ability to prioritize recall for at-risk groups. SVMs achieved:
	- Depression: 62% accuracy, 47% recall, 21% precision
	- Arrest history: 62% accuracy, 53% recall, 36% precision
	- Suicide ideation: 80% accuracy, 57% recall, 16% precision
	- Macro F1 scores: 0.52–0.57 across tasks
	- SVMs prioritized recall, making them useful for early flagging of at-risk individuals.

**Key findings:**
- Parental care and early support were more predictive of adult well-being than purely clinical childhood factors.
- Childhood adversity (e.g., being jumped, witnessing violence) increased risk for negative adult outcomes, but strong parental support mitigated these effects.
- The models performed best at identifying rare but critical outcomes (like suicide ideation), even with some tradeoff in precision.

**Limitations:**
- Predicting mental health is inherently complex; survey data and two timepoints can’t capture every factor.
- Results are most generalizable to the U.S. population.

---

## 🚀 Features

- **Workflow:** Reproducible research with Jupyter Notebooks
- **Data Cleaning & Processing:** Variable selection, encoding, and preprocessing
- **Statistical Analysis:** Correlation, regression, and hypothesis testing
- **Machine Learning Models:** Random Forest Regression, SVM Classifier
- **Visualizations:** Matplotlib & Seaborn for charts

---



## ⚡ Quick Start

1. **Clone the repository:**
	```bash
	git clone https://github.com/alyssaqle/COGS-108---Longitudinal-Mental-Health-Analysis.git
	cd COGS-108---Longitudinal-Mental-Health-Analysis
	```
2. **Install dependencies:**
	```bash
	pip install -r requirements.txt
	```
3. **Open the notebooks:**
	- Launch Jupyter:
	  ```bash
	  jupyter notebook
	  ```
	- Or use VS Code's built-in notebook support.
4. **Run the analysis:**
	- Start with the [Final Project Notebook](Notebooks/FinalProject_Group055_SP25.ipynb) for the complete workflow and results.

---




## 📂 Project Structure

```
COGS-108---Longitudinal-Mental-Health-Analysis/
├── Data/                         # Data folders from Add Health data source (e.g., DS0001 and DS0022 used in this project)
│   └── ...
├── Notebooks/                    # All project notebooks by phase
│   ├── ProjectProposal_Group055_SP25.ipynb   # Project proposal and planning
│   ├── DataCheckpoint_Group055_SP25.ipynb    # Data cleaning and preparation
│   ├── EDACheckpoint_Group055_SP25.ipynb     # Exploratory data analysis
│   └── FinalProject_Group055_SP25.ipynb      # Main analysis notebook
├── requirements.txt              # Python dependencies
└── README.md
```

---


## 📓 Project Workflow & Notebooks

The project is organized into four main Jupyter Notebooks, each corresponding to a phase of the class project:

- **ProjectProposal_Group055_SP25.ipynb**: Project proposal and planning (Phase 1)
- **DataCheckpoint_Group055_SP25.ipynb**: Data cleaning and preparation (Phase 2)
- **EDACheckpoint_Group055_SP25.ipynb**: Exploratory data analysis (Phase 3)
- **FinalProject_Group055_SP25.ipynb**: Complete analysis and final results (Phase 4)

Each notebook was submitted for feedback at the end of its phase, with improvements incorporated before moving to the next stage. **For the full, definitive analysis and results, open and run the [Final Project Notebook](Notebooks/FinalProject_Group055_SP25.ipynb).**

---


## 📊 Data Sources

This project uses the National Longitudinal Study of Adolescent to Adult Health (Add Health) public-use dataset, including:

- Early-life factors: breastfeeding duration, parental care, involvement in hobbies
- Adult outcomes: mental health diagnoses, depressive symptoms, counseling usage
- Waves 1 and 4: adolescence → adulthood progression

---


## 📈 Results

- **Random Forest Regressor:** Used for its ability to capture complex, nonlinear relationships and rank feature importance. Provided modest predictive power, with best R² = 0.13 for expected education level (edu_exp_a).
- **SVM Classifiers:** Chosen for their robustness in high-dimensional, imbalanced data and ability to prioritize recall for at-risk groups. Achieved 62–80% accuracy, recall up to 57% for identifying at-risk individuals (depression, arrest history, suicide ideation).
- These models were selected to balance interpretability, predictive power, and the need to flag at-risk individuals even when positive cases are rare.
- Findings show stronger predictive links between parental care and adult well-being than for purely clinical outcomes.

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
