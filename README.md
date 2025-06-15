# Exploratory Data Analysis (EDA) of the Titanic Dataset

## Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover key insights about passenger survival patterns. The analysis focuses on demographic, socioeconomic, and social factors that influenced survival rates during the Titanic disaster.

The dataset is sourced from the `seaborn` library's built-in Titanic dataset and is analyzed using Python libraries such as `pandas`, `seaborn`, `numpy`, and `matplotlib`.

---

## Dataset Description
The Titanic dataset contains information about passengers aboard the RMS Titanic, including attributes such as:

- **survived**: Survival status (0 = No, 1 = Yes)
- **pclass**: Passenger class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **sex**: Gender of the passenger
- **age**: Age of the passenger
- **sibsp**: Number of siblings/spouses aboard
- **parch**: Number of parents/children aboard
- **fare**: Ticket fare
- **embarked**: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- **class**: Passenger class (categorical)
- **who**: Passenger category (man, woman, child)
- **adult_male**: Whether the passenger is an adult male (True/False)
- **deck**: Deck of the ship
- **embark_town**: Town of embarkation
- **alive**: Survival status (yes/no)
- **alone**: Whether the passenger was traveling alone (True/False)

The dataset contains **891 rows** and **15 columns**, with some missing values (e.g., in `age` and `deck`) that were handled during the analysis.

---

## Key Findings

### 1. Demographic Insights
- **Gender**: Females had a significantly higher survival rate than males, likely due to the "women and children first" evacuation policy.
- **Age Groups**:
  - Children (age ≤ 12) had the highest survival rates.
  - Adults (18–40 years) had moderate survival rates.
  - Older passengers (60+ years) had lower survival chances.

### 2. Socioeconomic Insights
- **Passenger Class (Pclass)**:
  - 1st-class passengers had significantly higher survival rates than those in 2nd or 3rd class, likely due to better access to lifeboats.
- **Fare**:
  - Higher ticket fares correlated with higher survival rates, as wealthier passengers were often in 1st class with better safety measures.

### 3. Family and Social Connections
- **Family Size**:
  - Passengers with small families (1–3 members) had higher survival rates.
  - Large families (5+ members) faced challenges in coordinating and accessing lifeboats, leading to lower survival rates.
- **SibSp and Parch**:
  - Passengers traveling alone had lower survival rates compared to those with companions.

### 4. Embarkation Point
- Passengers embarking at **Cherbourg (C)** had the highest survival rates.
- **Southampton (S)** passengers had moderate survival chances.
- **Queenstown (Q)** passengers had the lowest survival rates.

### 5. Correlation Analysis
- A strong positive correlation exists between `fare` and `survived`, highlighting the role of economic status in survival.
- A slight correlation between `pclass` and `fare` underscores the advantages of higher-class passengers.

### 6. Final Observations
- **Survival Trends**: Gender, age, socioeconomic status, and embarkation point were major determinants of survival.
- **Disparities**: Females and 1st-class passengers were significantly more likely to survive.
- **Data Completeness**: Missing values (e.g., in `age`) were handled through imputation to ensure robust analysis.

---

## Repository Structure
- **Exploratory_Data_Analysis_Titanic.ipynb**: The Jupyter Notebook containing the complete EDA, including data loading, cleaning, visualizations, and insights.
- **README.md**: This file, providing an overview of the project and key findings.

---

## Dependencies
To run the analysis, install the following Python libraries:
```bash
pip install pandas seaborn numpy matplotlib
```

The analysis was performed using:
- Python 3
- Jupyter Notebook
- pandas
- seaborn
- numpy
- matplotlib

---

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/titanic-eda.git
   ```
2. Navigate to the project directory:
   ```bash
   cd titanic-eda
   ```
3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open and run the `Exploratory_Data_Analysis_Titanic.ipynb` notebook in Jupyter:
   ```bash
   jupyter notebook Exploratory_Data_Analysis_Titanic.ipynb
   ```

---

## Recommendations for Future Analysis
1. **Predictive Modeling**:
   - Use machine learning models (e.g., Logistic Regression, Random Forest) to predict survival based on these insights.
2. **Detailed Behavioral Studies**:
   - If time-series or sequence-based data becomes available, analyze the evacuation process to understand survival dynamics better.
3. **Feature Engineering**:
   - Create interaction terms (e.g., `pclass` and `sex`) or non-linear transformations of `fare` to enhance predictive models.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
For questions or feedback, feel free to reach out via [GitHub Issues](https://github.com/your-username/titanic-eda/issues).
