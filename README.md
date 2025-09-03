# NFLPA Survey Analysis (Python + Power BI)

This project cleans and restructures the NFLPA player survey data with Python (Google Colab) and visualizes it in Power BI to surface team strengths/weaknesses, year-over-year changes, and league trends.

---

## 📊 Project Overview
The NFLPA surveys players each season about facilities, staffing, travel, and leadership.  
Traditional outputs are dense letter-grade grids, which make it hard to quickly spot strengths and weaknesses.  
This project reimagines the presentation by:

- **Cleaning and transforming** the NFLPA survey data in Python (Google Colab)
- **Converting** letter grades to numeric scores (0.0–4.3 GPA-style)
- **Visualizing** results in an interactive Power BI dashboard
- **Highlighting** top/bottom teams, most improved, and category leaders

---

## 📂 Repository Contents

```
nflpa-survey-analysis/
│
├── data/
│   ├── NFLPA Survey Data.xlsb              # Raw multi-year survey data
│   ├── cleaned_nflpa_survey.csv            # Processed wide-format dataset
│   └── nflpa_survey_long_format.csv        # Processed long-format dataset
│
├── notebooks/
│   ├── NFLPA_Survey_Data_Cleaning.ipynb    # Data cleaning & transformation
│   └── NFLPA_PDF_Pages.ipynb               # PDF parsing / supplementary work
│
├── dashboard/
│   └── NFLPA Survey Analysis.pbix          # Power BI dashboard file
│
├── docs/
│   └── Merged Report Draft 2.pdf           # Full written report
│
├── README.md
└── LICENSE
```


---

## ⚙️ How to Use

### 1. Running the Notebooks
- Open `NFLPA_Survey_Data_Cleaning.ipynb` in **Google Colab** or **Jupyter Notebook**
- Install required Python packages (`pandas`, `numpy`, etc.)
- Run all cells to:
  - Clean column names and standardize categories
  - Convert letter grades to numeric scores
  - Generate wide and long format datasets for visualization
- Outputs:
  - `cleaned_nflpa_survey.csv`
  - `nflpa_survey_long_format.csv`

### 2. Viewing the Dashboard
- Download `NFLPA Survey Analysis.pbix`
- Open in **Power BI Desktop**
- Use slicers to explore:
  - League-wide category comparisons
  - Year-over-year changes
  - Team-specific strengths & weaknesses

### 3. Reading the Report
- `docs/Merged Report Draft 2.pdf` contains:
  - Executive summary
  - Methodology
  - Key findings
  - Category overviews
  - Full team report cards

---

## 📌 Key Insights from the 2024 Season
- **Top Performers:** Miami Dolphins, Minnesota Vikings, Atlanta Falcons
- **Most Improved:** Los Angeles Chargers, Atlanta Falcons, Washington Commanders
- **Common Trends:**
  - Strength staff & locker rooms score consistently high across the league
  - Ownership and family support vary widely between teams
  - Investments in facilities and communication correlate with higher player satisfaction

---

## 📑 Data Sources
- [NFLPA Report Cards 2023](https://nflpa.com/nfl-player-team-report-cards-2023)  
- [NFLPA Report Cards 2024](https://nflpa.com/nfl-player-team-report-cards-2024)  
- [NFLPA Report Cards 2025](https://nflpa.com/report-cards/2025)  

---

## 📜 License
This project is released under the MIT License.  
You are free to use, modify, and distribute the code with attribution.  
Please review the NFLPA’s own terms if redistributing raw data.

---

## 🚀 Future Work
- Automate yearly data ingestion
- Add more advanced DAX measures for deeper Power BI insights
- Create a public, interactive Power BI web link
