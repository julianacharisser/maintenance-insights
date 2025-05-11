# Exploratory Data Analysis on Halliburton Maintenance Logs 

This notebook explores 9 years of maintenance incident data to uncover high-impact issues, downtime trends, and root causes. The analysis helps identify where Halliburton is losing the most machine time—and how better categorization, design changes, or proactive maintenance can improve outcomes.

---

## 🧠 Key Insights & Visualizations

### 📉 Insight 1: Downtime is Concentrated

> Just 5 problems cause **75%** of all machine downtime hours.

- 🛑 The top culprit: `Axis is Noisy` alone caused **1,511 hours** lost—over **30%** of all recorded downtime.
- Visual: **Bar chart** of Top 5 Problem Codes by Machine Hours Lost.

![Top 5 Problem Codes](path/to/top5_bar_chart.png)

---

### 🔁 Insight 2: Axis Issues Are a Pattern

> Axis-related problems appeared **12 times**, with unusually high total downtime.

- Suggests a chronic design or maintenance flaw.
- Opportunity for targeted intervention or redesign.
- Visual: **Scatterplot** of Machine Hours Lost by Abnormality ID, highlighting Axis-related outliers.

![Outlier Scatter](path/to/axis_outliers.png)

---

### ⏱️ Insight 3: Resolution Time Is Long for Some Issues

> `Digital Readout Problem` had the **highest median resolution time** and **inconsistent durations**.

- Over **50%** of cases flagged as safety-related.
- Nearly all involve machine downtime.
- Visual: **Bar chart** of Median Resolution Time by Problem Code.

![Resolution Time](path/to/median_resolution_bar.png)

---

### 🗃️ Insight 4: Poor Categorization Adds Risk

> Incidents logged as `Problem Not Listed` had long resolution times—despite being vague.

- Indicates a documentation issue.
- Better problem code tagging could enable faster triage and root cause analysis.
- Visual: **Bar chart** of Top Unstructured Categories by Time Lost.

![Problem Not Listed](path/to/problem_not_listed_chart.png)

---

## 🧩 Next Steps

This EDA supports model training, dashboard development, and strategic maintenance recommendations. Key follow-ups:

- Use results to define labels/features for machine learning.
- Inform redesign or preventive maintenance programs.
- Improve technician note structure and issue tagging standards.
