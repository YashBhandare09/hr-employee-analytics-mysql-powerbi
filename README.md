# hr-employee-analytics-mysql-powerbi
HR Employee Data Analysis and Visualization using MySQL &amp; Power BI


<img width="1601" height="903" alt="Screenshot (175)" src="https://github.com/user-attachments/assets/4a317228-47b4-4421-87a4-27fb2cca31a8" />



---

## Data Used
- Dataset: HR employee data with over 22,000 records spanning the years 2000 to 2020.
- Data Cleaning & Analysis: MySQL Workbench
- Data Visualization: Power BI

---

## Data Cleaning & Analysis Process
The raw HR dataset was cleaned and prepared using MySQL:
1. Column Renaming – Updated ï»¿id to emp_id for clarity.
2. Date Standardization – Converted birthdate, hire_date, and termdate into proper DATE format.
3. Invalid Data Handling – Replaced blank or invalid termination dates with NULL.
4. Age Calculation – Added a calculated age column.
5. Data Filtering – Excluded employees under 18 and those with unrealistic ages or future termination dates.

---

## Business Questions Answered
1. Gender breakdown of employees in the company.
2. Race/ethnicity breakdown.
3. Age distribution.
4. Headquarters vs. remote workforce distribution.
5. Average length of employment for terminated employees.
6. Gender distribution by department and job title.
7. Distribution of job titles.
8. Department with the highest turnover rate.
9. Distribution of employees by state.
10. Employee count change over time.
11. Tenure distribution per department.

---

## Summary of Findings
- The workforce is male-dominated, with males representing a higher proportion across most departments.
- White employees form the largest racial group, while Native Hawaiian and American Indian are the least represented.
- Youngest employee: 20 years, oldest employee: 57 years.
- Age group distribution:
  - 25–34 years: Largest group
  - 35–44 years: Second largest
  - 55–64 years: Smallest group
- Most employees are based at headquarters rather than remote locations.
- Average length of employment for terminated employees is approximately 7 years.
- Gender distribution across departments is relatively balanced, though skewed slightly toward males.
- Marketing has the highest turnover rate, followed by Training.
- Lowest turnover rates are in Research & Development, Support, and Legal departments.
- The majority of employees are located in Ohio.
- Net employee count has shown a steady increase over the years.
- Average departmental tenure is around 8 years:
  - Highest: Legal and Auditing
  - Lowest: Services, Sales, and Marketing

---

## Limitations
- 967 records with negative ages were excluded (only employees aged 18 and above considered).
- 1,599 records with future termination dates were excluded (only termination dates ≤ current date used).
