# Hospital Patient Analytics Dashboard

An interactive **Power BI** dashboard that analyses hospital patient admissions by gender, medical condition, admission type, test results, hospital and time.

## Objective

To understand patient admission patterns and give hospital management a quick, filterable overview of:

- How many patients are admitted, and how this changes over time
- Patient mix by gender, medical condition and admission type
- Distribution of test results
- Which hospitals handle the most admissions

## Tools Used

- **Power BI Desktop**: data modelling, DAX measures, visuals
- **Dataset:** Hospital patient admission data from kaggle

## Dashboard Features

**KPI cards**

| Metric | Value |
|---|---|
| Total Admissions | 54,966 |
| Female Patients | 27,470 |
| Male Patients | 27,496 |
| Unique Patients | 40,235 |

**Visuals**

- Gender-wise patient distribution (pie chart)
- Patient count by medical condition (donut chart)
- Patient distribution by admission type (column chart)
- Patient admission trend over time (line chart)
- Hospital-wise total admissions (table)
- Patient distribution by test results (bar chart)

**Slicers / filters:** Date of Admission, Admission Type, Gender, Medical Condition

## Key Insights

- **Gender is almost evenly split:** about 50.02% female and 49.98% male.
- **Medical conditions are evenly spread:** Arthritis, Diabetes, Hypertension, Obesity, Cancer and Asthma each account for roughly 16.5% to 16.8% of patients.
- **Admission types are close in volume:** Elective (18.5K), Urgent (18.4K) and Emergency (18.1K).
- **Test results are balanced:** Abnormal (18.4K), Normal (18.3K) and Inconclusive (18.2K).
- **Admissions peaked between 2020 and 2023** at around 10K+ per year. The sharp fall in 2024 likely reflects an incomplete year of data.
- **Unique patients (40,235) are fewer than total admissions (54,966),** which means many patients were admitted more than once.

## How to Use

1. Download the `.pbix` file from this repository.
2. Open it in **Power BI Desktop**.
3. Use the slicers at the top to filter by date, admission type, gender or medical condition.


