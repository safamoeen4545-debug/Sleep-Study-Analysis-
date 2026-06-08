# 😴 Sleep Study Analysis – Phone Use & Daytime Tiredness

## 📌 Project Overview

Most people assume that if they sleep 7–8 hours, they’re fine.  
But does **phone use before bed** secretly steal your energy – even when you sleep the same number of hours?

This project analyzes survey data from 100+ individuals to uncover the relationship between:

- 📱 Phone use within 30 minutes of falling asleep  
- ⏰ Total sleep hours (weeknights)  
- 😴 Daytime tiredness (self‑reported on a 1–5 scale)  
- 🍳 Breakfast habits  

**Key question:**  
*Do phone users report higher tiredness at every sleep duration?*

---

## 📊 Key Findings

| Insight | Result |
|---------|--------|
| Phone before bed → higher tiredness | **+27%** average tiredness compared to non‑users |
| Even with same sleep hours | Phone users are **consistently more tired** at every sleep level (<6h, 6‑7h, 7‑8h, 8h+) |
| Only **42%** feel they get enough sleep | Majority are sleep‑deprived |
| Breakfast eaters | Report **lower tiredness** scores |

**Most eye‑catching chart:**  
Clustered column chart showing tiredness by `PhoneTime` (Yes/No) across four `SleepGroup` buckets.

---

## 📁 Data Source

**File:** `SleepStudyData.csv` (provided in this repo)  
**Rows:** ~100 responses  
**Columns:**  
- `Enough` – Do you think you get enough sleep? (Yes/No)  
- `Hours` – Average sleep hours on a weeknight  
- `PhoneReach` – Sleep with phone within arm's reach? (Yes/No)  
- `PhoneTime` – Use phone within 30 min of falling asleep? (Yes/No)  
- `Tired` – Daytime tiredness (1 = not tired, 5 = very tired)  
- `Breakfast` – Eat breakfast? (Yes/No)

> Dataset is clean with one missing `Hours` value (row 68) – removed during analysis.

---

## 🛠 Tools Used

- **Power BI Desktop** – Interactive dashboard & visualizations  
- **Excel** – Initial data cleaning and pivot table validation  
- **GitHub** – Project hosting  

---

## 📈 Analysis Steps

1. **Data Cleaning**  
   - Removed blank `Hours` row  
   - Created calculated columns in Power BI:  
     - `SleepGroup` (<6h, 6‑6.9h, 7‑7.9h, 8h+)  
     - `SleepDeprived` (Yes if Hours < 7)  
     - `TiredGroup` (Low, Medium, High)

2. **Measures Created**  
   - Average Hours  
   - Average Tiredness  
   - % Enough Sleep  
   - Total Respondents

3. **Visuals Built**  
   - KPI cards  
   - Tiredness by PhoneTime (bar chart)  
   - Tiredness by Breakfast (bar chart)  
   - Hours distribution (histogram)  
   - Average sleep hours by `Enough` (column chart)  
   - **Main insight chart:** Clustered column – `PhoneTime` vs `SleepGroup`

4. **Slicers Added**  
   - `Enough`, `SleepDeprived`, `Breakfast`, `PhoneTime`

---

## 🖼 Dashboard Preview

<img width="1381" height="744" alt="Screenshot 2026-06-08 232154" src="https://github.com/user-attachments/assets/551ce060-f8c9-461f-8d2c-057a43744b24" />


> *Full interactive dashboard available in Power BI file: `SleepStudyDashboard.pbix`*

---

## 📂 Repository Contents

| File | Description |
|------|-------------|
| `SleepStudyData.csv` | Raw survey data |
| `SleepStudyDashboard.pbix` | Power BI dashboard file |
| `Dashboard_Screenshot.png` | Static image of the dashboard |
| `README.md` | This file |

---

## 🔍 How to Replicate

1. Clone this repository  
2. Open `SleepStudyDashboard.pbix` in Power BI Desktop (free)  
3. Explore slicers and hover over charts for tooltips  
4. Modify measures or add new visuals as needed

---

## 💡 What I Learned

- Small datasets can tell powerful stories when you ask the right question.  
- A simple 2‑bar comparison (`PhoneTime` across `SleepGroup`) is more impactful than complex models.  
- Data storytelling is about **relatability** – everyone sleeps, everyone scrolls.

---

## 📢 Connect With Me

- [LinkedIn]https://www.linkedin.com/in/safa-moeen-90b7bb261/ 
E mail:safa.moeen4545@gmail.com

*If you found this analysis useful, give it a ⭐ and share your bedtime phone habit in the comments below!*
