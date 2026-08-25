Week 3: Python & Data Wrangling — Student Performance Data Cleaning
📌 Overview
This project is part of a Data Science internship (Week 3: Python & Data Wrangling). It demonstrates core data-cleaning and exploratory-analysis skills using Pandas, Matplotlib, and Seaborn on a messy student performance dataset.

🎯 Objective
Clean a messy dataset by:

Handling missing values
Filtering rows based on conditions
Creating new derived columns
Visualizing key insights
🗂️ Dataset
messy_student_data.csv — a synthetic student performance dataset containing realistic data-quality issues:

Missing values across multiple columns
Inconsistent text formatting (e.g. Male, male, M)
Duplicate rows
Out-of-range values (e.g. scores above 100 or negative)
Mixed date formats
🛠️ Tools & Libraries
Python 3
Pandas
NumPy
Matplotlib
Seaborn
Jupyter Notebook
🧹 Data Cleaning Steps
Removed duplicate rows
Standardized text fields (name casing, gender labels, city names)
Converted invalid entries to NaN and filled missing values using median/mode
Clipped out-of-range scores and attendance to a valid 0–100 range
Parsed and standardized inconsistent date formats
✨ Feature Engineering
Total_Score — sum of Math and Science scores
Average_Score — mean of the two subject scores
Grade — letter grade (A–F) derived from average score
Pass_Fail — pass/fail status based on average score
🔍 Row Filtering
Students with attendance ≥ 75%
Top performers with an average score ≥ 75
📊 Visualizations
Bar chart: average score by grade
Histogram: distribution of average scores
Boxplot: score spread by gender
Count plot: pass vs fail distribution
📁 Project Structure
├── Week3_Data_Wrangling.ipynb   # Main notebook with full analysis
├── clean_and_analyze.py         # Script version of the notebook
├── messy_student_data.csv       # Raw, uncleaned dataset
├── cleaned_student_data.csv     # Final cleaned dataset
├── chart_avg_score_by_grade.png
├── chart_score_distribution.png
├── chart_score_by_gender.png
├── chart_pass_fail_count.png
└── README.md
🚀 How to Run
pip install pandas numpy matplotlib seaborn
jupyter notebook Week3_Data_Wrangling.ipynb
📈 Key Outcomes
Reduced missing values across all columns from a raw dataset to zero
Standardized inconsistent categorical and date data
Generated actionable insights through visual analysis of student performance
