# 📊 NHIS 2023: Disability and Employment Analysis Using SAS

This project uses SAS 9.4 to analyze the 2023 National Health Interview Survey (NHIS) dataset, focusing on the relationship between sensory disabilities (vision and hearing) and employment status among U.S. adults aged 18–64. The analysis supports policy evaluation and public health recommendations aimed at improving workforce equity for individuals with disabilities.

---

## 🧠 Project Goals

- Identify how vision and hearing disabilities affect employment status
- Control for demographic and socioeconomic covariates
- Generate weighted national estimates using complex survey design
- Provide reproducible SAS code for public health research

---

## 📁 Repository Contents

| File | Description |
|------|-------------|
| [`nhis_disability_employment.sas`](./nhis_disability_employment.sas) | SAS script with full data cleaning, variable derivation, and analysis |
| `Appendice_YueYan.docx` | Original project appendix with annotated SAS code and project notes |
| `README.md` | Project overview and usage instructions |

---

## 🔍 Data Source

- **Dataset**: [2023 NHIS – Adult Public Use File](https://www.cdc.gov/nchs/nhis/data-questionnaires-documentation.htm)
- **Sample Size**: 29,522 total; 19,781 working-age adults included in analysis
- **Key Variables**:
  - Employment status (`Employed`)
  - Vision disability level (`Vision`)
  - Hearing disability level (`Hearing`)
  - Covariates: age, sex, education, ethnicity, region, workload, etc.
  - Survey design: `PSTRAT`, `PPSU`, `WTFA_A`

---

## 🛠 Methods & Techniques

- Data import and transformation (`PROC IMPORT`, `DATA`, `IF`, `FORMAT`)
- Descriptive statistics (`PROC MEANS`, `PROC FREQ`)
- Weighted estimates using complex survey design:
  - `PROC SURVEYFREQ`
  - `PROC SURVEYMEANS`
  - `PROC SURVEYLOGISTIC`
- Bivariate and multivariate analysis
- Adjusted odds ratios for disability-employment associations

---

## 📈 Key Findings

- Adults with **vision or hearing disabilities** were significantly less likely to be employed.
- After adjustment, individuals with **severe vision impairment** had **reduced odds of employment** compared to those with no impairment.
- The project highlights the need for accessible employment opportunities and targeted workforce support services.

---

## 🚀 How to Use

1. **Clone or download this repository**  
   ```bash
   git clone https://github.com/yourusername/nhis-disability-employment-sas.git
2. **If you use this code or analysis as a reference, please cite:
   ```bash
   Yue Yan, Baylor University, 2025
   NHIS 2023 – Disability and Employment Analysis Using SAS
