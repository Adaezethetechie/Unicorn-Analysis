# 🦄 Global Unicorn Companies Analysis (Power BI)

## 📌 Project Overview

This project provides a comprehensive, end-to-end Power BI analysis of global unicorn companies (privately held startups valued at over $1 billion). It explores industry distribution, funding-to-valuation ROI, geographical performance, and investor activity.

The dashboard processes data for 1,074 unicorns across 15 distinct industries, representing a combined valuation of $3.711 trillion and total funding of $591.82 billion. By focusing on robust data quality verification, transformation, and visual design, this project serves as a showcase of advanced data analysis and business intelligence techniques.

## 🛠️️ Data Preparation & ETL (Power Query)

!(Power Query Snapshot)[
To ensure accuracy for downstream DAX formulation and data modeling, extensive data cleaning and transformation were performed within the Power Query Editor. The ETL workflow included:

* **Text Standardization:** Applied `Trimmed Text` to remove invisible trailing/leading whitespace and utilized multiple `Replaced Value` steps to strip currency symbols and special characters.


* **Financial Unit Conversion:** Created custom logic to dynamically convert string-based financial identifiers (handling both millions "M" and billions "B") into a standardized, usable numeric scale for `Valuation` and `Funding`.


* **Date Parsing & Logic:** Utilized `Extracted Year` on the `Date Joined` column to isolate the exact year unicorn status was achieved.


* **Metric Engineering:** Engineered a custom column to calculate the "Years to $1B" metric by comparing the founding year to the year joined.


* **Data Type Structuring:** Explicitly defined data types across the dataset and structured the final table alphabetically by company to optimize performance.



## 📊 Dashboard Design & Data Modeling

The reporting layer was designed to provide interactive, executive-level insights using varied visual elements:

* **Geospatial Visualization:** An interactive global map plotting the Total Funding Received by Country.


* **Time-Intelligence & Trends:** Area charts tracking the timeline of unicorn creation and YoY growth metrics.


* **Matrix & Scatter Plot Analysis:** Matrix visuals for deep dives into investor portfolios and a scatter plot detailing Valuation Distribution across sectors.


* **DAX Measure Formulation:** Formulated custom measures to calculate ROI Multipliers, YoY Growth (82.3%), and Average Years to $1B dynamically.



## 💡 Key Business Insights

### High-Level KPIs

* **Total Unicorns:** 1,074.


* **Distinct Industries:** 15.


* **Global Valuation:** $3.711 Trillion.


* **Global Funding:** $591.82 Billion.


* **Average Time to Unicorn Status:** 7 years.



### Timeline of Unicorn Creation

Unicorn creation accelerated dramatically over the last decade, with a peak YoY growth of 82.3%.

* **2018:** 103 new unicorns.


* **2019:** 104 new unicorns.


* **2020:** 108 new unicorns.


* **2021:** 520 new unicorns (Historical peak).


* **2022:** 116 new unicorns.



### Industry & ROI Performance

* **Fastest to $1B:** Auto & Transportation averages 5 years to reach unicorn status, followed closely by AI and Hardware at 6 years.


* **Highest ROI:** The Fintech sector demonstrates a strong overall ROI Multiplier of 2.82, with individual standouts like *1047 Games* in Internet Software & Services achieving a 15.75 ROI multiplier.



### Regional & Investor Landscape

* **Regional Timelines:** Time-to-valuation varies significantly by region. For example, African Fintechs average 3 years to reach $1B, while South American Mobile/Telecommunications take up to 20 years.


* **Top Investors by Portfolio Valuation:**
* **Sequoia Capital:** $228B across 47 unicorns.


* **Accel:** $216B across 60 unicorns.


* **Andreessen Horowitz:** $213B across 52 unicorns.


* **Khosla Ventures:** $184B across 21 unicorns.


* **Insight Partners:** $150B across 47 unicorns.





## 📂 Project Structure

```text
├── Data/
│   ├── Unicorn_Companies.csv      # Raw dataset
│   └── Data_Dictionary.csv        # Dataset schema and descriptions
├── Dashboard/
│   └── Solution.pbix              # Fully functional Power BI file
├── Exports/
│   └── Solution.pdf               # Static export of dashboard pages
└── README.md                      # Project documentation

```

## 🚀 Usage & Target Audience

This repository demonstrates a complete, professional data analysis workflow. It is designed for:

* **Recruiters & Hiring Managers:** To evaluate my proficiency in Power BI, Power Query (M), DAX, and dashboard architecture.
* **Venture Capital Analysts:** To explore industry ROI, regional growth trends, and investor dominance.
* **Startup Founders:** To benchmark average timelines for reaching a $1 billion valuation based on industry and location.
