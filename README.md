🛳 Titanic-EDA-Project
📌 Project Overview

This project is part of my Elevvo Internship (Task 2: Exploratory Data Analysis).
The dataset is taken from the famous Kaggle Titanic: Machine Learning from Disaster
 challenge.

The goal of this task is to analyze passenger data and uncover key insights into survival patterns using Python, Pandas, Matplotlib, and Seaborn.

📊 Dataset Details

Source: Kaggle Titanic Dataset

File Used: train.csv

Shape: 891 passengers × 12 features

Target Variable: Survived (0 = Did not survive, 1 = Survived)

🔍 Data Preprocessing

Handled missing values:

Age (~20% missing) → imputed with median.

Cabin (~77% missing) → too sparse, created new feature HasCabin.

Embarked → only 2 missing values, filled with mode.

Created new engineered features:

FamilySize = SibSp + Parch + 1

HasCabin (1 if cabin available, 0 otherwise)

📈 Key EDA Insights
Univariate Analysis

Survival Rate: ~38% overall.

Gender: Females survived at ~74% vs ~19% for males.

Passenger Class: Survival higher in 1st > 2nd > 3rd class.

Age: Children (<15) had slightly better odds of survival.

Embarked: Passengers from port C had better survival chances.

Bivariate Analysis

Gender + Class: Women in 1st and 2nd class had the highest survival, men in 3rd class the lowest.

Family Features: Small families (2–4 members) had better survival chances than solo travelers or very large groups.

Correlation Heatmap

Survived strongly correlated with:

Negative correlation with Sex (male = 0, female = 1).

Positive correlation with Pclass.

SibSp and Parch weak individually, but combined into FamilySize showed clearer survival trends.

✅ Key Takeaways

Women and children first: They had higher survival rates.

Class mattered: Wealthier passengers had priority for safety.

Families: Small families had an advantage compared to being alone.

Insights align with the historical narrative of the Titanic disaster.

🛠️ Tools & Libraries

Python

Pandas

NumPy

Matplotlib

Seaborn
