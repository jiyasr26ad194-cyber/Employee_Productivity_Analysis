# Employee Attendance and Productivity Analysis

> **Spreadsheet Case Study | Data Analysis | Google Sheets / Microsoft Excel**

## 1. Case Study Title
**Employee Attendance and Productivity Analysis**

## 2. Problem Statement
An IT company maintains employee attendance and monthly productivity records. The HR department wants to identify employees with poor attendance, compare department-wise productivity, and analyze the relationship between attendance and productivity.

## 3. Objectives
- Calculate average attendance and total tasks completed.
- Identify the maximum and minimum number of tasks completed.
- Classify employees as Excellent, Satisfactory, or Poor based on attendance.
- Identify employees with attendance below 75%.
- Compare productivity across Development, Testing, and HR.
- Explore the relationship between attendance and tasks completed using charts and summary statistics.

## 4. Dataset Description
The dataset contains **12 employees** and five original fields:
- **Employee ID:** Unique employee identifier.
- **Name:** Employee name.
- **Department:** Development, Testing, or HR.
- **Attendance (%):** Monthly attendance percentage.
- **Tasks Completed:** Number of tasks completed during the month.

An additional calculated field, **Attendance Category**, classifies attendance as:
- **Excellent:** 90% and above.
- **Satisfactory:** 75%–89%.
- **Poor:** Below 75%.

The dataset is provided in [`Employee_Data.csv`](Employee_Data.csv).

## 5. Spreadsheet Functions Used
| Function | Purpose |
|---|---|
| `AVERAGE()` | Calculates average employee attendance. |
| `SUM()` | Calculates the total number of tasks completed. |
| `MAX()` | Finds the maximum tasks completed by an employee. |
| `MIN()` | Finds the minimum tasks completed by an employee. |
| `COUNT()` | Counts numeric employee records using the attendance or task column. |
| `IF()` | Assigns an attendance category based on the defined thresholds. |

**Example attendance classification formula** (assuming attendance is in `D2`):

```excel
=IF(D2>=90,"Excellent",IF(D2>=75,"Satisfactory","Poor"))
```

## 6. Data Analysis Techniques Performed
- Sorted employees by tasks completed in descending order.
- Filtered employees whose attendance was below 75%.
- Grouped employees by department.
- Applied conditional formatting to highlight attendance below 75%.
- Prepared a department-wise productivity summary using average tasks completed.

## 7. Charts and Visualizations
- **Bar chart:** Compares average tasks completed by department.
- **Pie chart:** Shows employee distribution across departments.
- **Histogram:** Displays the distribution of employee attendance.
- **Scatter plot:** Examines the relationship between attendance percentage and tasks completed.
- **Heat map:** Uses conditional formatting to show department-wise productivity patterns.

The dashboard preview is available at [`Screenshots/Dashboard.png`](Screenshots/Dashboard.png). The editable workbook, including the dataset, calculated fields, summary, and charts, is [`Employee_Productivity_Analysis.xlsx`](Employee_Productivity_Analysis.xlsx).

## 8. Important Observations
- The average employee attendance is **85.08%**.
- The employees completed **411 tasks** in total.
- The maximum number of tasks completed by one employee is **48**, by **Indhu** from **Development**.
- The minimum number of tasks completed is **20**.
- **2 employees** have poor attendance (below 75%): **Charan, Gokul**.
- **Development** has the highest average productivity at **38.20 tasks per employee**.
- The attendance–productivity correlation is approximately **0.82**, indicating a strong positive relationship in this sample. This is an association and does not prove that attendance alone causes higher productivity.

### Department-wise Productivity Summary

| Department | Employees | Total Tasks | Average Tasks per Employee |
|---|---:|---:|---:|
| Development | 5 | 191 | 38.20 |
| Testing | 4 | 143 | 35.75 |
| HR | 3 | 77 | 25.67 |

## 9. Conclusion
The analysis shows that Development has the highest average task completion among the three departments. Two employees fall below the attendance threshold of 75% and may need support. Attendance and task completion have a strong positive association in this dataset, although other factors such as task complexity, workload, resources, and individual roles can also influence productivity.

The HR department can use these findings to review attendance concerns, understand department-level performance, and provide appropriate support while considering the nature and quality of work—not only the number of tasks completed.

## 10. Google Sheets Sharing Link
**Add your Google Sheets link here:** `[Paste the view-access link]`

Before publishing, replace this placeholder with your actual Google Sheets URL and confirm that the link permissions allow the intended viewers to access it.

---

## Repository Contents
```text
Employee-Productivity-Analysis/
├── README.md
├── Employee_Productivity_Analysis.xlsx
├── Employee_Data.csv
├── Observations_and_Conclusion.md
└── Screenshots/
    └── Dashboard.png
```

## How to Use
1. Open `Employee_Productivity_Analysis.xlsx` in Microsoft Excel or upload it to Google Sheets.
2. Review the employee data, formulas, department summary, and charts.
3. Add your Google Sheets sharing URL in the section above.
4. Upload the files to a GitHub repository.
