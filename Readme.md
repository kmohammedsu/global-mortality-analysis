# Global Mortality Analysis

This project explores global mortality patterns using country-level data on healthcare, governance, and economic indicators. The goal is to understand the key factors driving differences in mortality rates across countries and to build models that can interpret or predict these outcomes.

## Objectives

- Identify relationships between mortality rates and socio-economic indicators such as healthcare infrastructure, health expenditure, corruption index, GDP, and happiness.
- Perform clustering to group countries with similar profiles.
- Use Decision Trees and Support Vector Regression (SVR) to model mortality rates.
- Create visualizations that offer global insights into health outcomes.

---

## Project Structure

```bash
├── Data/                     # Cleaned and reference datasets
├── Data Preprocesing/       # Preprocessing and feature engineering notebook
├── Notebooks/               # EDA, ML models (clustering, decision tree, SVR)
├── Visualizations/          # Output PNG charts from EDA
├── requirements.txt         # Python environment dependencies
└── README.md                # You're here!
```

---

##  Datasets Used

- **Global Mortality Data** (1990–2019): Possibly from WHO or GBD
- **Country Indicators**:
  - Hospital beds per 1000 people
  - Physicians per 1000 people
  - Public health expenditure
  - GDP per capita
  - Corruption index
  - Happiness score
- **Country reference list** to standardize naming across datasets

> Final cleaned data: `Final_Dataset_Cleaned.csv`

---

##  Methodology

1. **Data Preprocessing**
   - Cleaned and merged multiple datasets
   - Standardized country names using `pycountry`
   - Aggregated multi-year data for simplified analysis

2. **Exploratory Data Analysis (EDA)**
   - Visualized key trends and correlations
   - Focused on average values per country for interpretability

3. **Unsupervised Learning**
   - Performed clustering to group countries by mortality profiles
   - Possibly used PCA/SVD for dimensionality reduction

4. **Decision Tree**
   - Built regression tree to explain how indicators affect mortality
   - Extracted interpretable decision rules

5. **Support Vector Regression (SVR)**
   - Built predictive model for mortality rate
   - Applied scaling and model evaluation

---

##  How to Run

1. **Clone this repo**  
   `git clone https://github.com/kmohammedsu/global-mortality-analysis.git`

2. **Install dependencies**  
   (Recommended: Use virtual environment)  
   `pip install -r requirements.txt`

3. **Run Jupyter notebooks in order**:
   - `Data Preprocesing/02_data_preprocessing.ipynb`
   - `Notebooks/01_eda.ipynb`
   - `Notebooks/03_Unsupervised Learning.ipynb`
   - `Notebooks/04_Decision_Trees.ipynb`
   - `Notebooks/05_SVR.ipynb`

---

## Visualizations

Output charts include:
- Mortality rate distribution
- Beds/Physicians vs Mortality
- GDP vs Happiness vs Mortality
- Corruption index impact
- Public health expenditure comparison

See `Visualizations/` folder.


---

##  Team Members

- **Khaja Moinuddin Mohammed**
- **Prasanth Gururaj**
- **Sanjay Ramesh Kannan**
- **Sowmya Polagoni**
- **Venkat Saketh Kommi**

---


