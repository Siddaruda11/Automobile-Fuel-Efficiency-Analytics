# Automobile Fuel Efficiency Analytics with AI

Data Analytics with AI project submitted as part of the **IBM SkillsBuild Data
Analytics with AI Academic Internship Program**, conducted by BharatCares in
association with AICTE.

## Project Description

This project analyzes technical specifications of 398 cars (model years
1970-1982) — cylinders, engine displacement, horsepower, weight,
acceleration, model year and origin — to understand which factors most
strongly affect fuel efficiency (MPG). The goals are to:

1. Perform exploratory data analysis (EDA) on vehicle specifications and
   fuel efficiency trends.
2. Train regression models (Linear Regression and Random Forest) to
   predict a car's MPG from its specifications.
3. Translate the findings into recommendations for automotive design.

## Dataset

- **Name:** Auto MPG (UCI Machine Learning Repository)
- **Rows:** 398
- **Columns:** `mpg`, `cylinders`, `displacement`, `horsepower`,
  `weight`, `acceleration`, `model_year`, `origin`, `car_name`

## Technologies Used

- Python 3
- pandas, numpy — data manipulation
- matplotlib, seaborn — data visualization
- scikit-learn — Linear Regression, Random Forest Regressor
- Jupyter Notebook

## Project Structure

```
├── Siddaruda_AutoMPGAnalytics.ipynb   # Main analysis notebook
├── auto-mpg.csv                       # Dataset
├── requirements.txt                   # Python dependencies
└── README.md                          # This file
```

## Setup / Run Instructions

1. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd <repo-folder>
   ```
2. (Optional) Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Launch the notebook:
   ```bash
   jupyter notebook Siddaruda_AutoMPGAnalytics.ipynb
   ```
5. Run all cells (Cell → Run All).

## Key Findings

- **Weight, engine displacement, horsepower and cylinder count** are all
  strongly negatively correlated with MPG.
- **Average fuel efficiency improved steadily from 1970 to 1982**,
  reflecting industry-wide response to the oil crisis and tightening
  emissions standards.
- **Weight** is the single strongest predictor of fuel efficiency.
- A Random Forest Regressor achieved an **R² score of ~0.91** on the
  held-out test set, outperforming Linear Regression (R² ~0.85).

## Recommendations

1. Prioritize weight reduction in vehicle design for the biggest MPG gains.
2. Optimize engine displacement and cylinder count for efficiency.
3. Track year-over-year efficiency trends to guide continuous improvement.
4. Use the trained model for early-stage MPG estimates during design.

## Author

Siddaruda Satyappa Mantur — BCA student, IBM SkillsBuild Data Analytics
with AI Academic Internship (BharatCares x AICTE), 2026.
