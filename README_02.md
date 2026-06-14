# PRODIGY_DS_02 — Titanic EDA & Data Cleaning

**Prodigy InfoTech | Data Science Internship | Task 02**

## Objective
Perform data cleaning and exploratory data analysis (EDA) on the Titanic dataset to explore relationships between variables and identify patterns in survival rates.

## Dataset
Titanic — Machine Learning from Disaster | [Kaggle](https://www.kaggle.com/c/titanic/data)  
891 passengers · 12 features

## Data Cleaning Steps
| Issue | Treatment |
|---|---|
| Age — 177 missing (19.9%) | Filled with median grouped by Pclass + Sex |
| Embarked — 2 missing | Filled with mode (port 'S') |
| Cabin — 687 missing (77.1%) | Dropped (too sparse to impute) |
| Duplicates | None found |

## Feature Engineering
- `FamilySize` = SibSp + Parch + 1
- `IsAlone` = 1 if FamilySize == 1
- `AgeGroup` = Child / Teen / Adult / Middle-aged / Senior

## Key Insights
- Women survived at nearly 3× the rate of men — "women and children first" is statistically confirmed
- 1st class passengers had the highest survival rate; 3rd class the lowest
- Small families (2–4 members) survived better than solo travelers or large groups
- Age and fare are right-skewed; class and fare are strongly correlated

## Visualizations
- Overall survival rate
- Survival by gender
- Survival by passenger class
- Age distribution by survival
- Survival by class & gender (grouped bar)
- Fare distribution by class (box plot)
- Survival by family size

## Tech Stack
Python 3 · pandas · numpy · matplotlib · Jupyter Notebook

## Files
```
PRODIGY_DS_02/
├── PRODIGY_DS_02.ipynb       # Main notebook
├── titanic.csv               # Dataset
├── task02_visualization.png  # Full dashboard
└── README.md
```

## Author
**Sargun (Divsargun Kaur)** — B.Tech Textile Technology, NIT Jalandhar (Batch 2029)  
[LinkedIn](https://linkedin.com/in/divsargunkaur) · [GitHub](https://github.com/divsargun1803)
