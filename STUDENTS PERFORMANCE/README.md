# Students Performance Analysis (SQL + Power BI)

An end-to-end data analysis project on student academic performance. Data was cleaned and explored using **MySQL**, then visualised in an interactive **Power BI** dashboard.

## Objective

To understand which factors affect students' final results and give teachers and management a quick, filterable overview of:

- Overall pass and fail numbers
- Average grades across student groups
- Impact of previous failures, study time and absences on performance
- Student distribution by gender and age

## Tools Used

| Tool | Purpose |
|---|---|
| **MySQL** | Data cleaning, validation and exploratory analysis |
| **Power BI Desktop** | Data modelling, DAX measures and dashboard |

**Dataset:** `student-mat` (student performance in Mathematics), 395 records. Add the source link here.

Key columns: `school`, `sex`, `age`, `address`, `famsize`, `Pstatus`, `Medu`, `Fedu`, `traveltime`, `studytime`, `failures`, `absences`, `higher`, `G1`, `G2`, `G3` (G3 = final grade).

## Part 1: SQL Analysis

The full script is in `studentsperformance.sql`.

**Data cleaning and validation**
- Checked total row count
- Checked for duplicate records across all key columns
- Checked for NULL values in important columns
- Checked for extra spaces using `TRIM`
- Standardised text values using `UPPER`

**Exploratory analysis**
- Student count by gender, age and study time
- Average age and average final grade (`G3`)
- Average final grade by gender, study time, failures and absences
- Pass/fail split using `CASE WHEN G3 >= 10 THEN 'pass' ELSE 'fail'`
- Number of students aiming for higher education (`higher`)
- Highest final grade and number of students with full marks (`G3 = 20`)
- Performance categories: **Excellent** (G3 ≥ 15), **Average** (G3 ≥ 10), **Needs Improvement** (G3 < 10)

## Part 2: Power BI Dashboard

**KPI cards**

| Metric | Value |
|---|---|
| Total Students | 395 |
| Pass Percentage | 67.09% |
| Average Grade | 10.42 |
| Pass Students | 265 |
| Failed Students | 130 |

A student is counted as **Pass** if the final grade (G3) is 10 or above.

**Visuals**
- Pass vs Fail students (pie chart)
- Average grade by previous failures (line chart)
- Gender-wise student count (donut chart)
- Average final grade by gender (column chart)
- Student count by age (treemap)
- Student count by study time (bar chart)

**Slicers:** Study Time, Gender, Age

## Key Insights

- **About 67% of students passed** (265 of 395), and 130 students (32.91%) failed.
- **Previous failures strongly lower grades.** The average grade drops from about 11 for students with no past failures to about 6 for those with 2 to 3 failures.
- **Gender split:** 208 female (52.66%) and 187 male (47.34%) students. Male students have a slightly higher average final grade.
- **Most students are aged 15 to 18.** Ages 16 (104) and 17 (98) are the largest groups.
- **Study time level 2 is the most common** (about 200 students), followed by level 1 (about 105). Levels 3 and 4 have far fewer students.

## How to Use

1. Open `studentsperformance.sql` in MySQL Workbench and run the queries on the `student-mat` table.
2. Download the `.pbix` file and open it in **Power BI Desktop**.
3. Use the slicers at the top to filter by study time, gender or age.
