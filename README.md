# global-tech-layoff and power BI dashboard
An interactive power BI dashboard analyzing global tech layoffs with dynamic ranking metrics and time intelligence parameters


📌 Project Overview
This project focuses on analyzing global tech industry layoff trends using Power BI for interactive dashboard visualization and data modeling. The objective is to uncover key business and economic insights related to layoff patterns across various sectors, geographical locations, company stages, and time periods. The project demonstrates how data analytics can transform complex workforce reduction data into meaningful visualizations that support strategic decision-making and market analysis.


 🎯 Objectives  
* Perform data cleaning, transformation, and preprocessing using Power Query.  
* Implement dynamic ranking metrics, time-intelligence parameters, and DAX measures.  
* Analyze layoff distributions across different industries, countries, and funding stages.  
* Identify peak layoff periods and employment trend patterns over time.  
*Build an interactive Power BI dashboard featuring matrix tables and geographic bubble map visualizations.  
*Generate actionable insights regarding the global tech market landscape.


🛠️ Technologies Used  
* Power BI Desktop  
* Power Query  
* DAX (Data Analysis Expressions)  
* Data Modeling & Visualization


📁 Project Structure
Global-Tech-Layoffs-Analysis/
│
├── tech_layoffs_dataset.csv          # Dataset 
├── layoffs_data_cleaning.ipynb       # Python EDA & preprocessing script
├── global_tech_layoffs_powerbi.pbix  # Power BI Dashboard file
└── README.md                         # Project documentation


📁 Dataset Description
*The dataset contains global tech industry workforce reduction and layoff information, consisting of the following columns:  
*event_id: Unique identifier for each layoff event.  
*company: Name of the tech company undergoing workforce reductions.  
* hq_city: City where the company's headquarters is located.  
* country: Country of the company's headquarters.  
* industry: Business sector or domain of the company (e.g., Other, Retail, Consumer, Transport, Food, Media).  
* funding: Funding stage or status of the company (e.g., Post-IPO, Private Equity, Series B, Seed).  
* total_laid_off: Number of employees laid off in the event.  
*layoff: Percentage range or exact proportion of the workforce affected.  
* layoff_date: The specific date when the layoff occurred.  
* quarter: The financial/calendar quarter of the layoff event (e.g., 2025 Q2).  
* month: The month name corresponding to the layoff date.  
* month_num: Numeric representation of the month.
 

🧹 Data Preprocessing
The following preprocessing steps were performed:
* Checked for missing values across company records, funding stages, and layoff numbers.  
* Removed duplicate records to ensure data integrity.  
* Converted date columns into datetime format for accurate time-intelligence analysis.  
* Standardized categorical values (such as industry sectors and funding stages).  
* Corrected inconsistent values by removing trailing spaces and standardizing text formatting.  
* Verified data types for all columns prior to modeling.
* mass_layoff: Boolean flag indicating if it qualified as a large-scale or mass layoff.  
* ai_related: Boolean flag indicating whether the layoff was driven by or related to AI adoption/integration.  
* source_url: Reference link or source of the reported layoff data

📈 Exploratory Data Analysis (EDA)
The notebook includes analysis of:
* Total Layoffs Overview: Aggregate count of total employees laid off globally across all recorded companies.
* Layoffs by Industry: Sector-wise breakdown identifying which industries (e.g., Consumer, Retail, Tech, Healthcare, Finance) faced the highest workforce reductions.
* Layoffs by Country: Geographic distribution analyzing which countries and regions experienced the most severe layoff impacts.
* Layoffs by Stage: Analysis based on company funding stages (e.g., Post-IPO, Series A–J, Seed, Startup) to see which company maturity level was hit hardest.
* Top Layoff Companies: Identification of the top companies with the absolute highest number of layoffs.
* Funds Raised vs. Layoffs Correlation: Exploring the relationship between capital raised prior to layoffs and the scale of job cuts.
* Yearly & Monthly Layoff Trends: Time-series analysis tracking how tech layoffs surged, peaked, and fluctuated over time (e.g., 2022–2026).
* Percentage Laid Off Distribution: Examining whether companies opted for partial downsizing or 100% shutdowns (going out of business).
* Location-based City/Hub Analysis: Deep dive into specific tech hubs (e.g., SF Bay Area, Bangalore, New York, London) affected.
* Layoff Seasonality Patterns: Investigating if specific quarters or months exhibited spikes in workforce reductions.

  
📊 Power BI Dashboard

The dashboard includes:

KPI Cards

* Total Companies: Total count of unique companies that implemented layoffs.  
* Total Laid Off: Cumulative number of employees impacted globally.  
* Max Layoffs (Single Event): The single highest number of employees laid off by a single company in one instance.
* Total Funds Raised: Aggregate capital raised by the affected companies prior to downsizing.

  
Visualizations

* Layoffs Over Time (Line Chart): Dynamic timeline showing monthly/yearly progression of tech layoffs with drill-down capabilities.
* Layoffs by Industry (Bar / Column Chart): Clean comparative breakdown of total layoffs distributed across diverse sectors.
* Geographic Bubble Map: Interactive map displaying layoff concentrations globally, with bubble sizes proportional to the magnitude of layoffs.
* Top 10 Layoff Companies (Ranked Bar Chart): Horizontal bar chart highlighting the largest corporate downsizing events.
* Funds Raised vs. Total Laid Off (Scatter Plot): Correlation plot showing how funding size relates to layoff volume.
* Company Stage Breakdown (Donut / Treemap Chart): Visual share of layoffs categorized by company funding rounds.
* Interactive Slicers & Filters: Global filters for Year, Country, Industry, and Funding Stage to make the dashboard fully interactive and dynamic for recruiters.

🎛️ Interactive Filters


The dashboard includes interactive slicers and filters for:

* Country (Filter layoffs by specific countries or global regions)
*Industry (Isolate sectors like Consumer, Retail, Finance, or Tech)
* Funding Stage (Analyze trends across Post-IPO, Seed, Series A–J, etc.)
* Year / Date Range (Track fluctuations across specific years and quarters)
* Company Size / Stage (Filter by startup maturity or enterprise level)

  
🔍 Key Insights

* Sector Vulnerability: The Consumer and Retail industries experienced the highest total volume of layoffs during economic contraction periods.
* Funding vs. Layoffs: Companies that raised massive venture capital (Series C+) prior to the downturn accounted for a significant share of total employee layoffs.
* Geographic Concentration: The United States (specifically the SF Bay Area and New York tech hubs) recorded the highest percentage of total global layoffs.
* Data Cleaning Impact: Standardizing company names, removing null values, and handling missing funding amounts significantly improved the accuracy of industry-wise aggregations.
* Peak Downsizing Window: The highest spikes in workforce reductions occurred during late 2022 and throughout 2023, followed by stabilization phases.

  
📸 Dashboard Preview
Add screenshots of your Power BI dashboard here.  
Example:<img width="1920" height="1200" alt="image" src="https://github.com/user-attachments/assets/388512eb-b02f-423b-9d3a-b0764bf72ad2" />

# 🌍 Global-Layoffs-Analysis-Dashboard

## 📺 How to Run the Project

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/global-layoffs-analysis-dashboard.git](https://github.com/your-username/global-layoffs-analysis-dashboard.git)


2. Install Required Libraries

pip install pandas numpy matplotlib seaborn openpyxl

3. Open the Notebook

jupiter notebook layoffs_data_cleaning_eda.ipynb

4. Open Power BI Dashboard


Open the .pbix file using Microsoft Power BI Desktop to explore the interactive visualizations.


📌 Results
The project successfully demonstrates:
* Data cleaning and preprocessing of global layoff records
* Exploratory Data Analysis (EDA) using Python (Pandas, Seaborn)
* Identification of peak layoff periods, hardest-hit industries, and geographic trends
* Interactive dashboard development using Power BI with drill-downs and filters
These analyses help stakeholders monitor market trends, identify impacted sectors, and understand modern workforce shifts.
[global layoff.pdf]

---

## 🚀 Future Enhancements

* Layoff Forecasting using Machine Learning Models (e.g., Time Series Forecasting)
* Company Risk Scoring & Vulnerability Analysis
* Regional & Geographic Impact Mapping
* Live Data Pipeline for Real-time Dashboard Integration
* Automated Weekly Layoff Report Generation

---

## 📚 References

* Python Documentation: https://docs.python.org/
* Pandas Documentation: https://pandas.pydata.org/
* NumPy Documentation: https://numpy.org/
* Matplotlib Documentation: https://matplotlib.org/
* Seaborn Documentation: https://seaborn.pydata.org/
* Microsoft Power BI Documentation: https://learn.microsoft.com/power-bi/

---

## 🧑‍💻 Author

**Rizana Sherin**

Global Tech Layoffs Data Analysis using Python & Power BI Dashboard Project






