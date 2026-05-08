# HR-Metrics-Dashboard
Interactive Power BI dashboard for analyzing employee attrition, workforce demographics, job satisfaction, and HR performance metrics.
## Dashboard Preview

<img width="1421" height="950" alt="image" src="https://github.com/user-attachments/assets/944503f3-7e12-498a-b06f-ee03c3b477af" />


---

## Project Overview

This dashboard provides insights into:
- Employee attrition trends
- Department-wise attrition
- Job satisfaction ratings
- Employee age distribution
- Education field analysis
- Gender-based attrition

---

## Key Metrics

| Metric | Value |
|---|---|
| Overall Employees | 1470 |
| Attrition Count | 237 |
| Attrition Rate | 16.12% |
| Active Employees | 1233 |
| Average Age | 37 |

---

## Tools & Technologies

- Power BI Desktop
- Power Query
- DAX
- Excel Dataset

---

## DAX Measures

```DAX
Overall Employees = COUNT(Employee[EmployeeID])

Attrition Count =
CALCULATE(
    COUNT(Employee[EmployeeID]),
    Employee[Attrition] = "Yes"
)

Attrition Rate =
DIVIDE([Attrition Count], [Overall Employees], 0)
```

---

## Insights

- Sales department shows the highest attrition.
- Employees aged 25–34 form the largest workforce group.
- Attrition is higher among younger employees.
- Job satisfaction differs across job roles.

---

## Project Structure

```bash
HR-Analytics-Dashboard/
│
├── HR_Analytics.pbix
├── dataset/
├── screenshots/
└── README.md
```

---

## How to Use

1. Clone the repository
2. Open the `.pbix` file in Power BI Desktop
3. Refresh the dataset if needed
4. Explore the dashboard using filters and slicers

