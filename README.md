# ABC Call Volume Trend Analysis

##  Project Overview
This project explores **Customer Experience (CX) analytics** by analyzing inbound call center data from Insurance Company. The goal is to identify call volume trends, optimize agent allocation, and improve the overall customer experience.

The dataset provided spans **23 days** and includes:
- Agent details (name and ID)
- Queue time
- Call time and duration
- Call status (Answered, Abandoned, Transferred)

The analysis will help address key pain points such as high call abandonment rate and insufficient night-time support.

---

##  Business Understanding
Customer satisfaction is a core business priority, and call centers play a vital role in shaping that experience. A 30% abandon rate reflects poorly on the brand and highlights inefficiencies in agent staffing.

Our objective is to:
- Identify peak call times
- Propose efficient manpower allocation plans
- Ensure 90% of calls are answered both during the day and night shifts

---

##  Dataset Description
- **Source:** Internal dataset from ABC Insurance Company
- **Duration:** 23 days
- **Scope:** Inbound calls

### Key Columns:
| Column Name     | Description                              |
|----------------|------------------------------------------|
| Agent Name     | Name of the call center agent             |
| Agent ID       | Unique identifier for the agent           |
| Queue Time     | Time the customer waited before connection|
| Call Time      | Timestamp of the call                     |
| Call Duration  | Length of the call                        |
| Call Status    | Answered, Abandoned, or Transferred       |

---

##  Data Analytics Tasks

### 1️. Average Call Duration by Time Bucket
- **Goal:** Calculate the average duration of calls in each hourly time bucket (e.g., 9-10 AM).
- **Output:** Table or chart summarizing average durations.

### 2️. Call Volume Analysis
- **Goal:** Visualize the total number of calls per time bucket.
- **Output:** Bar or line graph showing call volume trends from 9 AM to 9 PM.

### 3️. Manpower Planning (Day Shift)
- **Goal:** Reduce call abandonment from 30% to 10%.
- **Method:**
  - Calculate total number of calls per time bucket.
  - Estimate required agents to answer 90% of those calls.
  - Apply efficiency assumptions (agent availability and utilization).

### 4️. Night Shift Manpower Planning
- **Goal:** Plan staffing from 9 PM to 9 AM based on projected 30% of daytime volume.
- **Output:** Full 24-hour manpower plan ensuring <10% abandon rate.

---

##  Assumptions
- Each agent works **6 days/week**
- Agents take **4 unplanned leaves/month**
- Work duration: **9 hours/day** (with 1.5 hours break)
- Productive call time: **60% of 7.5 hours = 4.5 hours/day**
- **30 days in a month**

These assumptions will inform agent availability and staffing requirements.

---

##  Tools Used
- **Excel:** Data cleaning, PivotTables, formula-based calculations
- **Charts & Graphs:** Line charts, bar graphs, scatter plots, combo charts
- **Formulas Used:**
  - `AVERAGEIF()`
  - `COUNTIF()`
  - `SUMIF()`
  - `VLOOKUP()` / `XLOOKUP()`

---

##  Deliverables
- Excel workbook with:
  - Cleaned and formatted dataset
  - All analysis with relevant visualizations
  - Agent staffing calculator (day + night shifts)
- Visual dashboard for:
  - Call volume
  - Call duration
  - Staffing needs per time bucket

---

##  Key Insights & Recommendations
- **Peak Hours:** Identify time slots with highest abandon rate
- **Staffing Strategy:** Suggest optimal number of agents to maintain SLA
- **Night Shift Coverage:** Plan realistic staffing based on extended service window

---

##  Repository Structure
```
ABC-Call-Volume-Trend-Analysis/
├──  Dataset/
│   └── ABC_Call_Data.csv
├──  Excel_Analysis/
│   └── ABC_Call_Volume_Dashboard.xlsx
├──  Visualizations/
│   ├── Call_Volume_Trend.png
│   ├── Avg_Call_Duration_By_Hour.png
│   └── Manpower_Planning_Summary.png
├──  README.md
└──  Insights_Summary.pdf
```

---



