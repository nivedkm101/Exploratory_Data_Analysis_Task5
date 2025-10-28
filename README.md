Titanic Dataset - Exploratory Data Analysis (EDA)

# 🚢 Titanic Dataset - Exploratory Data Analysis (EDA)

## 📘 Overview
This project performs **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover key patterns and insights related to passenger survival. 
It involves data cleaning, feature engineering, and visual analysis using **Python**, **Pandas**, **Matplotlib**, and **Seaborn**.

---

## 🧰 Tools & Libraries Used
- **Python**
- **Pandas** – Data manipulation
- **NumPy** – Numerical operations
- **Matplotlib** – Data visualization
- **Seaborn** – Statistical data visualization
- **Google Colab** – Notebook environment

---

## 📂 Dataset
**Source:** Titanic dataset (`train.csv`)  

**Key Features:**
| Column | Description |
|--------|-------------|
| Survived | Survival status (0 = No, 1 = Yes) |
| Pclass | Passenger class (1, 2, 3) |
| Sex | Gender of passenger |
| Age | Age of passenger |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Fare | Ticket fare |
| Embarked | Port of embarkation |
| Cabin / Ticket | Dropped during cleaning (too many missing values) |

---

## 🧹 Data Preprocessing Steps
1. **Handle Missing Values:**
   - `Age` filled with median.
   - `Embarked` filled with mode.
2. **Feature Engineering:**
   - Created `Family_size = SibSp + Parch`.
3. **Dropped Unnecessary Columns:**
   - Removed `Cabin`, `Ticket`, `SibSp`, and `Parch`.
4. **Standardized Column Names:**
   - Converted to lowercase and replaced spaces with underscores.
5. **Saved Cleaned Data:**
   - Exported as `Titanic_cleanned_task5.csv`.

---

## 📊 Visual Analysis & Observations

### 1️⃣ Pairplot
**Observation:**  
- Higher fares and smaller families had greater survival chances.  
- Survivors concentrated in high-fare regions.

### 2️⃣ Correlation Heatmap
**Observation:**  
- Positive correlation between `fare` and `survival`.  
- Negative correlation between `pclass` and `survival`.

### 3️⃣ Survival Count by Sex
**Observation:**  
- Females had a much higher survival count.  
- Gender played a major role in survival outcome.

### 4️⃣ Survival Rate by Sex
**Observation:**  
- Female survival rate ≈ 75%, Male ≈ 20%.  
- “Women and children first” pattern visible.

### 5️⃣ Survival Rate by Sex and Passenger Class
**Observation:**  
- Female 1st and 2nd class passengers had the highest survival.  
- Males in 3rd class had the lowest survival rate.

### 6️⃣ Distribution of Numerical Features
**Observation:**  
- **Age:** Mostly 20–40 years old.  
- **Fare:** Right-skewed — few very high fares.  
- **Family Size:** Mostly small families.

### 7️⃣ Boxplots (Age & Fare vs Survival)
**Observation:**  
- Survivors had lower median age and higher fare.  
- Fare strongly impacted survival probability.

### 8️⃣ Scatterplot (Age vs Fare by Survival)
**Observation:**  
- Survivors cluster at higher fare values.  
- Age less influential compared to fare.

### 9️⃣ Passenger Class Impact
**Observation:**  
- 1st class: Highest survival rate (~60–65%).  
- 3rd class: Lowest (~25%).  
- Class significantly affected survival.

---

## 📈 Key Findings
- **Gender** was the strongest survival predictor — females had much higher chances.  
- **Fare** and **class** were crucial socioeconomic indicators.  
- **Younger** passengers survived slightly more.  
- **Large families** had lower survival rates.  
- **No severe multicollinearity** between numerical features.

---

## 🧠 Conclusion
This analysis confirms that survival on the Titanic was highly influenced by **gender**, **class**, and **fare**.  
Women, first-class passengers, and those who paid higher fares had the best chances of survival.

---

## 💾 Output
- Cleaned dataset saved as: `Titanic_cleanned_task5.csv`
- EDA visualizations and analysis available in Google Colab notebook.

---

## 👤 Author
**Nived K M**  
📧 Email: nivedkm101@gmail.com  
🔗 GitHub: [github.com/nivedkm101](https://github.com/nivedkm101)  
💼 LinkedIn: [linkedin.com/in/nivedkm101](https://linkedin.com/in/nivedkm101)

---
## 📚 References
- Kaggle: [Titanic - Machine Learning from Disaster]([https://www.kaggle.com/c/titanic](https://www.kaggle.com/c/titanic/data?select=train.csv&utm_source=chatgpt.com))
- Seaborn & Matplotlib Documentation

---


