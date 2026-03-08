# Excel_FUNCTIONS

# 📊 Excel Functions — Practice Dataset Repository

> **By [DatawithRose](https://github.com/Rose-Armstrong)** 🌹
> 
> Free practice files for the **Excel Functions Tutorial Series** — as featured on YouTube and LinkedIn.

---

## 👋 Welcome!

This repository contains the **HR Employee Dataset** used across all 7 videos in the *DatawithRose Excel Functions Series*. Each folder corresponds to a tutorial day and includes:

- 📝 A **Practice File** — try the functions yourself before watching
- ✅ An **Answer File** — the completed version used in the tutorial

Whether you're a complete beginner or brushing up your skills, these files are designed to help you learn by doing!

---

## 📁 Repository Structure

```
Excel_FUNCTIONS/
│
├── Day 1/
│   ├── HR_Excel_Series_Dataset - Practice - Day 1.xlsx
│   └── HR_Excel_Series_Dataset - Answers - Day 1.xlsx
│
├── Day 2/
│   ├── HR_Excel_Series_Dataset - Practice - Day 2.xlsx
│   └── HR_Excel_Series_Dataset - Answers - Day 2.xlsx
│
├── Day 3/
│   ├── HR_Excel_Series_Dataset - Practice - Day 3.xlsx
│   └── HR_Excel_Series_Dataset - Answers - Day 3.xlsx
│
├── Day 4/
│   ├── HR_Excel_Series_Dataset - Practice - Day 4.xlsx
│   └── HR_Excel_Series_Dataset - Answers - Day 4.xlsx
│
├── Day 5/
│   ├── HR_Excel_Series_Dataset - Practice - Day 5.xlsx
│   └── HR_Excel_Series_Dataset - Answers - Day 5.xlsx
│
├── Day 6/
│   ├── HR_Excel_Series_Dataset - Practice - Day 6.xlsx
│   └── HR_Excel_Series_Dataset - Answers - Day 6.xlsx
│
│
└── README.md
```

---

## 📚 Tutorial Series Overview

| Day | Topic | Functions Covered | Video |
|-----|-------|-------------------|-------|
| Day 1 | Excel Foundation Functions | `SUM` `AVERAGE` `COUNT` `COUNTA` `COUNTBLANK` | [Watch](https://youtu.be/dW8OH2npQ90) |
| Day 2 | Logical Functions | `IF` `Nested IF` `IFS` | [Watch](https://youtu.be/635qmjRskq0) |
| Day 3 | Conditional Counting | `COUNTIF` `COUNTIFS` | [Watch](https://youtu.be/6WdPKvHac80) |
| Day 4 | Conditional Summing | `SUMIF` | [Watch](https://youtu.be/tsoe-g-4yOg) |
| Day 5 | Conditional Averaging | `AVERAGEIF` `AVERAGEIFS` | [Watch](https://youtu.be/fNCuvC9MODo) |
| Day 6 | Power Combos | `IF + COUNTIF` `IF + AND` | [Watch](https://youtu.be/l5eWMGpd-o8) |

---

## 🗂️ About the Dataset

All tutorials use a consistent **HR Employee Dataset** so you can follow along seamlessly across all 7 days.

### Dataset Columns

| Column | Description | Type |
|--------|-------------|------|
| `Emp_ID` | Employee identification number | Text |
| `Name` | Employee full name | Text |
| `Department` | HR, Finance, IT, Marketing, Operations, Sales | Text |
| `Gender` | Male / Female | Text |
| `Age` | Employee age | Number |
| `Join_Date` | Date of joining the company | Date |
| `Years_of_Service` | Tenure in years | Number |
| `Salary` | Annual compensation (USD) | Number |
| `Performance_Score` | Performance rating (1–5 scale) | Number |
| `Performance_%` | Performance percentage | Number |
| `Attendance_%` | Attendance percentage | Number |
| `Training_Hours` | Hours of training completed | Number |
| `Promoted` | Promotion status — Yes / No | Text |
| `City` | Work location | Text |
| `Status` | Active / Inactive employment status | Text |

### Dataset Size
- **Rows:** 50 employee records
- **Columns:** 15 fields
- **Departments:** 6 (HR, Finance, IT, Marketing, Operations, Sales)

---

## 🚀 How to Use These Files

**Step 1** — Navigate to the folder for the Day you are studying

**Step 2** — Download the **Practice File** first and attempt the exercises on your own

**Step 3** — Watch the corresponding YouTube tutorial if you get stuck

**Step 4** — Compare your work against the **Answer File** to check your results

**Step 5** — Experiment! Change the criteria, thresholds, and ranges to deepen your understanding

> 💡 **Tip:** Try completing the practice file BEFORE watching the video — you'll learn much faster that way!

---

## 📖 Quick Formula Reference

### Day 1 — Foundation Functions
```excel
=SUM(D3:D52)
=AVERAGE(E3:E52)
=COUNT(E3:E52)
=COUNTA(A3:A52)
=COUNTBLANK(A3:E52)
```

### Day 2 — IF & IFS
```excel
=IF(E3>3, "Valued", "Under")
=IF(D3>=90000,"High", IF(D3>=65000,"Mid", IF(D3>=45000,"Entry","Trainee")))
=IFS(E3>4.5,"Outstanding", E3>3.5,"Good", E3>2.5,"Average", TRUE,"Poor")
```

### Day 3 — COUNTIF & COUNTIFS
```excel
=COUNTIF(C3:C92, A4)
=COUNTIFS(C3:C52, A4, N3:N52, "Active")
=COUNTIFS(C3:C52, A4, D3:D52, "Female")
=COUNTIFS(C3:C52, A4, I3:I52, ">=4")
```

### Day 4 — SUMIF
```excel
=SUMIF(B:B, "East", C:C)
=SUMIF(B:B, E1, C:C)
=SUMIF(C:C, ">1000", C:C)
=SUMIF(A:A, "*Phone", C:C)
```

### Day 5 — SUMIF & SUMIFS
```excel
=SUMIF(C3:C52, "HR", H3:H52)
=SUMIFS(H3:H52, C3:C52, "HR", N3:N52, "Active")
=SUMIFS(H3:H52, C3:C52, "HR", D3:D52, "Female")
=SUMIFS(H3:H52, C3:C52, "HR", H3:H52, ">=75000")
```

### Day 6 — AVERAGEIF & AVERAGEIFS
```excel
=IFERROR(AVERAGEIF(C3:C52, "HR", H3:H52), "")
=IFERROR(AVERAGEIFS(K3:K52, C3:C52, "HR", M3:M52, "Active"), "")
=IFERROR(AVERAGEIFS(H3:H52, D3:D52, "Male", C3:C52, "HR"), "")
=IFERROR(AVERAGEIFS(H3:H52, D3:D52, "Female", C3:C52, "HR"), "")
```

### Day 7 — Power Combos
```excel
=IF(COUNTIF(B3:B52, B3)>1, "Duplicate", "Unique")
=IF(AND(E3<70, F3<85), "At Risk", "OK")
=IF(OR(E3<70, F3<85), "Review", "OK")
```

---

## 🔗 Connect with DatawithRose

Stay connected for more free Excel tutorials, tips, and resources!

| Platform | Link |
|----------|------|
| 🎥 YouTube | [DatawithRose](https://www.youtube.com/@DatawithRose) |
| 💼 LinkedIn | [LinkedIn](https://www.linkedin.com/in/rose-armstrong/) |
| 📝 Blog | [Blog](https://medium.com/@DatawithRose) |
| 🐙 GitHub | [github.com/Rose-Armstrong](https://github.com/Rose-Armstrong) |

---

## ⭐ Support This Work

If these files helped you learn Excel, please consider:

- ⭐ **Starring this repository** — it helps others find it!
- 👍 **Liking the YouTube videos** — it helps the channel grow
- 🔔 **Subscribing** — so you never miss a new tutorial
- 💬 **Sharing with a friend** who wants to learn Excel for free

---

## 📄 License

These practice files are free to use for **personal learning and educational purposes**.
Please credit **DatawithRose** if you share or reference this work. 🌹

---

*Made with 🌹 by DatawithRose — Empowering everyone to work confidently with data.*
