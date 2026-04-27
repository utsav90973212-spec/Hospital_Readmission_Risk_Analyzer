# 🏥 Hospital Readmission Risk Analyzer

> Identifying high-risk diabetic patients before discharge using data-driven risk scoring

**Author:** Utsav Raj | PGDM-BM | Aspiring Business Analyst  
**Tools:** Python | pandas | numpy | plotly | Google Colab  
**Dataset:** Diabetes 130-US Hospitals (1999–2008) — UCI Machine Learning Repository  

---

## 🎯 Business Problem

Hospital readmissions within 30 days trigger financial penalties under the **Hospital Readmissions Reduction Program (HRRP)**. Medicare penalizes hospitals for excessive readmission rates — making prevention a top priority.

**Core question:** Can we identify HIGH RISK patients BEFORE discharge so hospitals can intervene early?

---

## 📊 Dataset

- 101,766 patient encounters across 130 US hospitals
- 50 variables including age, diagnoses, medications, lab results
- 10 years of real clinical data (1999–2008)

---

## 🔬 Research Hypotheses Tested

| Hypothesis | Finding | Confirmed? |
|---|---|---|
| Older patients readmit more | Young adults (20-30) actually highest at 14.4% | ❌ Surprised! |
| More diagnoses = higher risk | 9+ diagnoses = >12% readmission rate | ✅ Confirmed |
| More medications = higher risk | 20+ medications = 11-16% elevated risk | ✅ Confirmed |
| Previous admissions predict risk | 3+ visits crosses 20% threshold | ✅ Strongest predictor |

---

## 🏆 Key Finding — Risk Scoring System

Built a rule-based risk scoring system using 4 clinical variables:

| Risk Level | Patients | Readmission Rate |
|---|---|---|
| LOW | 70,812 | 9.6% |
| MEDIUM | 24,415 | 14.0% |
| HIGH | 2,826 | **29.2%** |

**HIGH risk patients are 3x more likely to be readmitted than LOW risk patients.**

By focusing on just 2,826 HIGH risk patients (2.9% of total), hospitals can prevent the majority of penalty-triggering readmissions.

---

## 💡 Business Recommendations

1. **Implement pre-discharge risk screening** for all diabetic patients
2. **Stronger counseling for 20-30 age group** — highest surprise risk group
3. **Flag patients with 7+ diagnoses** for extended stay or mandatory follow-up
4. **Pharmacy review before discharge** for patients on 20+ medications
5. **Auto-flag patients with 3+ previous admissions** as HIGH RISK
6. **Assign care coordinator** to all HIGH risk patients for 30-day post-discharge monitoring

---

## 📁 Repository Structure

```
hospital-readmission-risk-analyzer/
├── Hospital_Readmission_Risk_Analyzer.ipynb  ← Complete analysis notebook
├── diabetic_data.csv                          ← Raw dataset
└── README.md                                  ← This file
```

---

## 🚀 How to Run

1. Open `Hospital_Readmission_Risk_Analyzer.ipynb` in Google Colab
2. Upload `diabetic_data.csv` to your Google Drive
3. Update the file path in Cell 2
4. Run all cells top to bottom

---

*This project was built as part of my Business Analytics learning journey*  
*transitioning from Law → Business Analytics through PGDM-BM program*
