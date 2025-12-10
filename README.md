#  Transport Ridership Forecasting  
A complete end-to-end data analysis and forecasting project using Python, Prophet, and Jupyter Notebook.

This project analyzes multi-year ridership data across several  transport routes, extracts insights, detects anomalies, and produces 7-day ridership forecasts. It includes a full EDA pipeline, forecasting models, visual dashboards, and structured reporting.

---

# Project Objectives  
- Perform Exploratory Data Analysis (EDA)  
- Identify trends, seasonality, and anomalies  
- Build 7-day forecasts using Facebook Prophet  
- Generate an automated insights dashboard  
- Export predictions, insights, and reports  
- Provide clear business-ready interpretations  

---

# Dataset Overview  
The dataset contains daily ridership counts for:

- **Local Route**  
- **Light Rail**  
- **Peak Service**  
- **Rapid Route**  
- **School**

Rows: ~1,900  
Columns: 7  
Time Span: Multiple years  

---

# Key Insights

1. Weekly Seasonality  
Ridership is consistently higher on weekdays and lower on weekends — especially for School and Peak Service routes.

2.Pandemic Impact (2020–2021)  
A major drop in ridership occurs during COVID-19 lockdown periods.

3. Post-Pandemic Recovery  
After 2022, ridership trends show recovery, especially in Local and Rapid Routes.

4. Route-Specific Patterns  
- **Local & Rapid:** High, stable usage  
- **Peak Service:** Office-hour dependent  
- **School:** Vacation-sensitive with strong dips  
- **Light Rail:** Steady moderate ridership  

5. Seasonal Dips  
Certain months show notable drops due to holidays, festivals, or school vacations.

---

# Insights Dashboard  
A 6-panel dashboard summarizes major insights:

- Overall multi-year trend  
- Weekday vs Weekend comparison  
- Monthly seasonality heatmap  
- Pandemic period analysis  
- Sudden drops / anomaly detection  
- Forecast preview  

 **Dashboard File:**  
`results/insights_images/dashboard_insights.png`

---

# Forecasting Model  

### Model Used: **Facebook Prophet**  
Prophet is ideal for business time-series because it:  
- Detects daily, weekly, yearly seasonality  
- Handles missing data  
- Adjusts for changing trends  
- Produces confidence intervals  

### Forecasts Generated For:
- Local Route  
- Light Rail  
- Peak Service  
- Rapid Route  
- School  

 Forecast Output Files:  
`results/forecast_<route>.csv`

---

# Evaluation Metrics  
Metrics used to assess forecasting performance:

- **MAE — Mean Absolute Error**  
- **RMSE — Root Mean Squared Error**  
- **MAPE — Mean Absolute Percentage Error**  

Metric files (if generated) stored in:  
`results/metrics/`

---

##  How to Run the Project

## Install Dependencies  
```bash
pip install prophet pandas numpy matplotlib seaborn scikit-learn
```

## Open the Notebook  
```bash
jupyter notebook notebooks/analysis_and_forecast.ipynb
```

## Run All Cells  
Executing the notebook will automatically:

- Load and preprocess the dataset  
- Generate all EDA visualizations  
- Build the insights dashboard  
- Train Prophet models  
- Export forecasts, charts, and summaries into the `results/` directory  

---

##  Reports Included

### Insight Report  
Detailed summary of insights, dashboards, and CSV analyses.  
**Path:** `reports/insight_report.md`

###  Technical Report  
Explains forecasting methodology, Prophet model reasoning, and evaluation.  
**Path:** `reports/technical_report.md`

---

##  Project Structure  

```
transport-forecast-project/
│
├── data/
│   └── Daily_Public_Transport_Passenger_Journeys_by_Service_Type_20250603.csv
│
├── notebooks/
│   └── analysis_and_forecast.ipynb
│
├── results/
│   ├── forecast_Local_Route.csv
│   ├── forecast_Light_Rail.csv
│   ├── forecast_Peak_Service.csv
│   ├── forecast_Rapid_Route.csv
│   ├── forecast_School.csv
│   │
│   ├── insights/
│   │   ├── weekday_vs_weekend_summary.csv
│   │   ├── monthly_avg_by_route.csv
│   │   ├── pandemic_impact_summary.csv
│   │   ├── largest_drops_summary.csv
│   │   └── auto_insights_summary.txt
│   │
│   └── insights_images/
│       ├── dashboard_insights.png
│       ├── overall_trend_all_routes.png
│       ├── weekday_vs_weekend.png
│       ├── monthly_heatmap.png
│       └── drops_annotation.png
│
├── reports/
│   ├── insight_report.md
│   └── technical_report.md
│
└── README.md
```

---

##  Why This Project Stands Out  

This project showcases real-world data science skills used in:

- Transportation & mobility analytics  
- Logistics & demand forecasting  
- Business operations & planning  
- Data science and ML engineering  

###  Strengths Highlighted:
- Advanced **time-series forecasting** using Prophet  
- **Seasonality, trend, and anomaly analysis**  
- Clean and structured **EDA workflow**  
- Professional **data visualizations and dashboards**  
- Reproducible, industry-standard **project structure**  
- Business-oriented, actionable **insights and reports**


