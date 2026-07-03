# Project-8-Python-For-Data-Analysis-Census
End-to-end EDA on India Census 2011 | Analyzing population, religion, workers &amp; education across 640 districts using Python, Pandas, Matplotlib &amp; Seaborn

# Data Analysis Project — India Census 2011

An end-to-end Data Analysis project on India Census 2011 district-level data, completed as part of the **Python for Data Analysis** course.

## 📌 Objective
Explore population distribution, religion breakdown, workforce participation, and education levels across 640 Indian districts using advanced Pandas operations.

## 📂 Dataset
- **Source:** CensusData.csv — India Census 2011
- **Records:** 640 districts
- **States:** 35
- **Features:** District_code, State_name, District_name, Population, Male, Female, Literate, Workers, Male_Workers, Female_Workers, Cultivator_Workers, Agricultural_Workers, Household_Workers, Hindus, Muslims, Christians, Sikhs, Buddhists, Jains, Secondary_Education, Higher_Education, Graduate_Education, Age_Group_0_29, Age_Group_30_49, Age_Group_50

## 🛠️ Tools & Libraries
| Library | Purpose |
|---|---|
| Pandas | Data analysis, groupby, styling, indexing |
| Matplotlib | Base plotting |
| Seaborn | Statistical visualizations |

## 🔧 Pandas Commands Covered
| Command | Purpose |
|---|---|
| `style.hide()` | Hide the DataFrame index for clean display |
| `style.set_caption()` | Add a title/heading above the DataFrame |
| `isin()` | Filter rows matching multiple values at once |
| `groupby().sum()` | Aggregate data by category |
| `set_index()` | Set a column as the DataFrame index |
| `add_suffix()` | Append a string to all column names |
| `add_prefix()` | Prepend a string to all column names |

## ❓ Analytical Questions

### Q1 — Hide the index of the DataFrame
Use `style.hide()` to display the DataFrame without the default numeric index.

### Q2 — Set a caption/heading on the DataFrame
Use `style.set_caption()` to add a descriptive title above the displayed table.

### Q3 — Show records for New Delhi, Lucknow, and Jaipur
Use `isin()` to filter multiple district values in a single clean expression.

### Q4 — State-wise Population & Religion Distribution
- **(A)** Total population per state using `groupby('State_name')['Population'].sum()`
- **(B)** Total count of each religion per state

### Q5 — Male Workers in Maharashtra
Filter for Maharashtra and sum `Male_Workers` — also demonstrated via `groupby()` for all states at once.

### Q6 — Set a column as the DataFrame index
Use `set_index('District_name')` to enable label-based `.loc[]` access.

### Q7 — Add Suffix and Prefix to column names
- **(7a)** `add_suffix('_2011')` — useful when merging multiple census years
- **(7b)** `add_prefix('census_')` — useful when merging with non-census datasets

## 📊 Analysis Structure
1. Imports & Setup
2. Load Dataset
3. First Look (head / tail)
4. Data Structure & Info
5. Missing Values Check
6. Descriptive Statistics
7. Analytical Questions (Q1 → Q7)
8. Visualizations
   - Univariate (Population Distribution + Boxplots)
   - Top States Bar Charts
   - Religion Distribution (Pie + Stacked Bar)
   - Bivariate (Population vs Workers/Literate)
   - Age Group Distribution
   - Correlation Heatmap · Pairplot
9. Key Insights

## 💡 Key Insights
- Uttar Pradesh is the most populous state, followed by Maharashtra and Bihar
- Hinduism represents ~80% of India's population nationally
- Maharashtra leads all states in Male Workers (32.6 million)
- Population and Workers are very strongly correlated across all districts
- India's 0–29 age group forms the largest demographic segment
- Female workforce participation is significantly lower than male across all states

## 🚀 How to Run
```bash
git clone https://github.com/ammarelsayed-2a/Project-8-Python-For-Data-Analysis-Census.git
cd Project-8-Python-For-Data-Analysis-Census
jupyter notebook "Project 8 Census.ipynb"
```

## 👤 Author
**Ammar Elsayed** — Python for Data Analysis | 2026  
[LinkedIn](https://www.linkedin.com/in/ammar-elsayed-ibrahim)
