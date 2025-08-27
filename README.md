


# Longitudinal Mental Health Analysis 🧠
---
## TL;DR: This project analyzes over 4,500 records from the Add Health study to examine how childhood emotional support influences adult mental health, using exploratory data analysis, Random Forest regression, and Support Vector Machine classification to identify predictive patterns and public health implications.

## ⭐ For a detailed explanation of the project, including the methodology and results, please refer to the [Final Project Notebook](Notebooks/FinalProject_Group055_SP25.ipynb).

---

## 👥 Authors

- Alexandro Merida Silva
- Adam Rolander
- Alyssa Le
- Enrique Aranda
- Hikari Gregersen
---

## 📝 Summary

What separates adults with strong mental health from those who struggle? 

That’s the question we set out to answer by analyzing longitudinal survey data from over 1,700 individuals in the Add Health study, tracking their journey from adolescence to adulthood.

Using statistical analysis and machine learning, we found that higher early-life emotional support—measured by parental care, breastfeeding duration, and involvement in hobbies—was strongly associated with better adult mental health outcomes.

- **Data cleaning**  
  - Started with **4,500+ Add Health participants**, reduced to **~1,700 complete cases** to avoid bias from missing data.  
  - Split into **childhood predictors** (parental care, grades, breastfeeding, violence, hobbies) and **adult outcomes** (depression, education, arrest, suicide ideation).  

- **Exploratory Data Analysis (EDA)**  
  - **Pairplots:** chosen to spot *correlations and clusters*. Showed family warmth variables clustered; more parental care → fewer depressive feelings.  
  - **Heatmap:** used to detect *redundancy and strong associations*. Revealed overlap (mother vs parents care) and negative links between violence and family warmth.  
  - **PCA:** applied to *reduce complexity* and highlight main drivers. Found family support and education expectations as key dimensions.  
  - **Bar charts:** chosen to make *group comparisons* clear. Showed higher parental care → lower depression and counseling.  

- **Modeling**  
  - **Random Forest Regression:** selected for *continuous outcomes*. Handles non-linearities and redundant predictors (seen in heatmap). Modest fit (best R² = 0.13), but ranked key predictors (grades, parental support).  
  - **Support Vector Machines (SVMs):** selected for *binary outcomes*. Works well with imbalanced data and lets us prioritize recall.  
    - Depression → 62% accuracy, 47% recall  
    - Arrest → 62% accuracy, 53% recall  
    - Suicide ideation → 80% accuracy, 57% recall  
    - Recall > precision by design → better for flagging at-risk individuals.  

- **Insights**  
  - Strong parental care → better adult mental health.  
  - Violence exposure → worse outcomes, but family support buffered some effects.  
  - Academic performance in adolescence → tied to education expectations in adulthood.  
  - Depression and suicide hardest to predict → too complex for limited survey data.  

- **Takeaway**  
  - Early emotional support has a **lasting impact** on adult outcomes.  
  - Even with modest accuracy, models gave evidence-backed insights that could guide **public health efforts** like parenting programs and violence prevention.  

- **Limitations**  
  - Predicting mental health is inherently complex; survey data and two timepoints can’t capture every factor.  
  - Results are most generalizable to the U.S. population.  

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
│   └── FinalProject_Group055_SP25.ipynb      # Main Final notebook
├── requirements.txt              # Python dependencies
└── README.md
```


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


## 🛠️ Technologies

- Python (Pandas, NumPy) for data processing
- Jupyter Notebooks for analysis and documentation
- Matplotlib, Seaborn for visualization
- scikit-learn for machine learning

---


## 📜 License

For academic use only. Dataset subject to Add Health terms of use.
