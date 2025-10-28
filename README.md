# Predicting Road Accident Risk
**Playground Series - Season 5, Episode 10 (Kaggle Competition)**  

This repository contains code and analysis for predicting the **risk of road accidents** using a machine learning approach.  
The dataset used in this competition was synthetically generated from a deep learning model trained on the **Simulated Roads Accident dataset**.  
The goal is to develop models that accurately estimate accident risk based on various road and environmental features.

---

## Dataset Description
The dataset for this competition (both train and test) was generated from a deep learning model trained on the Simulated Roads Accident dataset.  
Feature distributions are close to, but not exactly the same, as the original.  
You may use the original dataset to explore differences or test whether combining it with the competition data improves performance.

**Data files:**
- `train.csv` features + target (risk level)
- `test.csv` features only (for prediction)
- `sample_submission.csv` sample output format

---

## Project Objectives
1. Explore and visualize the dataset  
2. Engineer meaningful features  
3. Train and compare models (LightGBM, XGBoost, CatBoost, etc.)  
4. Optimize hyperparameters and improve validation performance  
5. Prepare submission file for Kaggle  

---

## Repository Structure
```
road/
│
├── data/             # Datasets (not uploaded)
├── notebooks/        # Jupyter notebooks for EDA and modeling
├── src/              # Python scripts (functions, training, utils)
├── app/              # Streamlit web app (optional)
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

---

## Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/amritorupam/road.git
cd road
```

###  2. Create a virtual environment (optional but recommended)
```bash
python -m venv venv
venv\Scripts\activate   # On Windows
# source venv/bin/activate   # On macOS/Linux
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

---

##  Model Development Steps
- **Exploratory Data Analysis (EDA):** Understand feature patterns and distributions  
- **Feature Engineering:** Handle missing values, encode categorical features, and scale numerical values  
- **Modeling:** Train LightGBM, XGBoost, and CatBoost models using K-Fold cross-validation  
- **Evaluation:** Track mean and standard deviation of fold scores  
- **Submission:** Generate predictions for the test dataset  

---

## Results & Observations
- Best performing model: *(to be updated)*  
- Validation RMSE/Accuracy: *(to be updated)*  
- Feature importance: Analyzed using SHAP and permutation importance  

---

## Streamlit App (Being Developed)
A simple web interface for predicting accident risk can be built using Streamlit:
```bash
streamlit run app/app.py
```

---

## Tools & Libraries
- Python 3.10+
- Pandas, NumPy, Scikit-learn
- LightGBM, XGBoost, CatBoost
- Matplotlib, Seaborn
- Streamlit (for app deployment)

---

## License
This project is licensed under the **MIT License**.

---

## Author
**Amrito Rupam Ghosh**  
Studying B.Tech CSE | Aspiring Machine Learning Engineer  
Kaggle: https://www.kaggle.com/amritorupamghosh
GitHub: https://github.com/amritorupam

---

**If you find this repository useful, please give it a star!**
