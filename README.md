# Student Result Analysis System

A simple data analysis project built with **Python**, **Pandas**, and **NumPy** that processes student academic records — computing totals, percentages, grades, pass/fail results, and generating basic statistical insights.

##  Overview

This project creates a dataset of 8 students with scores across 5 subjects (Math, Science, English, Computer, Social) and performs a full analysis : from raw scores to grades, results, and visualizations.

## Dataset

Each student record includes:

| Column | Description |
|---|---|
| `studentid` | Unique student ID |
| `Name` | Student name |
| `Age` | Student age |
| `Math`, `Science`, `English`, `Computer`, `Social` | Subject-wise marks |
| `Attendance` | Attendance percentage |
| `Gender` | Male / Female |

## Processing Steps

1. **Data Creation** — Builds the initial student dataset using a Pandas DataFrame and exports it to `student_info.csv`.
2. **Total Marks** — Sums marks across all 5 subjects.
3. **Percentage** — Calculates percentage based on total marks out of 5 subjects.
4. **Grade Assignment** — Assigns letter grades based on percentage:
   - `A+` ≥ 90
   - `A` 80–89
   - `B` 70–79
   - `C` 60–69
   - `F` < 60
5. **Pass/Fail Result** — A student **fails** if they score below 40 in *any* subject; otherwise they **pass**.
6. **Result Summary** — Counts of PASS vs FAIL using `groupby`.
7. **Ranking by Percentage** — Sorts students from topper to lowest scorer.
8. **Subject-wise Statistics**
   - Highest marks scored per subject
   - Average marks per subject
   - Easiest subject (highest average)
   - Hardest subject (lowest average)
9. **Filtering**
   - Students scoring ≥ 80%
   - Students with attendance below 75%
##  Tech used

- Python
- Pandas
- NumPy


## Output 

- `student_info.csv` — Exported dataset with all computed columns (Total, Percentage, Grade, Result, etc.)

