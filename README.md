# Netflix Data Analytics Dashboard (MySQL to Power BI)

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-00000F?style=for-the-badge&logo=mysql&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-CC292B?style=for-the-badge&logo=microsoftsqlserver&logoColor=white)

Interactive Power BI dashboard analyzing Netflix content trends, genres, ratings, countries, and release patterns using data visualization techniques.

##  Dashboard Features & Insights

The report is split into two specialized analytical views to balance high-level macro trends with micro-level detail:

### Page 1: Overview
*This view uncovers macroscopic content trends, release velocity, and geographical footprints.*
* **Shows Added by Date:** An area/line chart tracking the explosive growth of both Movies and TV Shows over time, pinpointing peak content acquisition periods (around 2018–2020).
* **Shows by Rating:** A stacked column chart breaks down volume by content maturity levels (e.g., TV-MA, TV-14, PG-13), segmented by media type.
* **Top 10 Genres:** Horizontal bar chart identifying major audience buckets, highlighting "International Movies" and "Dramas" as dominant library categories.
* **Geographical Distribution:** A dynamic global bubble map plotting global content availability and regional production concentrations.

### Page 2: Single Title View
*A granular search engine and decision-support view for individual content profiles.*
* **Interactive Dynamic Slicer:** Allows users to pick any specific Movie or TV Show (e.g., `#Roxy`).
* **KPI Cards:** Instant lookup fields displaying precise information for Release Year (2018) and Content Rating (TV-14).
* **Metadata Parsing:** Generates automated text blocks for show descriptions, specific genre tags ("Listed In"), Directors, and full Cast listings dynamically.
* **Contextual Mapping:** Synchronizes with the selection to highlight the exact country of origin or target market on a regional map layout.

---

## Technical Stack & Skills Demonstrated

* **Database Engine:** MySQL / SQL
* **BI Platform:** Power BI Desktop
* **Data Modeling:** Star Schema (Fact/Dimension table separation based on split tables visible in the data pane like `netflix_data_countries`, `netflix_cast`, etc.)
* **UI/UX Design:** Custom Canvas Grid Layout, Branded Color Theming (Netflix Red `#E50914` on Dark Gray `#141414`), Tooltips, and Interactive Page Navigation.

---

## 5. Repository Structure

```directory
├── Assets/                 # Dashboard screenshots used in documentation
├── Dashboard/              # Contains the .pbix file
│   └── Netflix_Data_Dashboard.pbix
└── Database_Scripts/       # SQL scripts for database creation and analysis
    ├── schema_setup.sql
    └── queries.sql
