📊 NEW DASHBOARD: SALARY ANALYSIS IN PORTUGAL (2015–2022)



📌 Overview

This project presents a dashboard analyzing the evolution of salaries in Portugal between 2015 and 2022.

The main goal was not to produce an exhaustive academic study, but to practice real ETL, build a clean data model, and create professional visualizations, working with challenging public data — just like in many real-world analytics projects.

The data was obtained from several public tables provided by Pordata, one of Portugal’s main statistical platforms.



📁 Data Sources

The tables used in this project were extracted from:

🔗 www.pordata.pt



Pordata was chosen because the more detailed public sources (such as INE, DGAEP, MTSSS and others) present a much higher level of complexity, including:

* Highly fragmented categories
* Repeated combinations of dimensions
* Unintuitive filters
* Truncated indicators
* Structural changes over the years
* Different granularities for similar variables



Standardizing data at this level would require a project dedicated exclusively to data cleaning and harmonization.

Even so, Pordata has some limitations:

* Rigid segmentation
* Unclear categories
* Gaps in recent years
* Incomplete series before 2015 and after 2022



For this reason, the analysis focuses on 2015–2022, the most consistent period.



🔧 ETL Process (Python)

The raw datasets went through a complete ETL pipeline:

* Cleaning and standardization of tables
* Selection of the correct indicators
* Filtering for mainland Portugal
* Removal of inconsistent or missing values
* Normalization of column structures
* Export of clean CSVs for modeling



Libraries used:

pandas, numpy, pathlib



🧩 Data Modeling (Power BI)

The model was built using a star schema, including:

* DimAno (Year Dimension)
* Fact tables for salaries by: sex, age, education level, professional group, sector, macro sector, minimum wage.



Additional steps included:

* Exclusion of incomplete years
* Standardization of relationships between tables
* Creation of DAX measures
* Harmonization of different granularities across fact tables



📊 Visualizations \& Key Insights

The dashboard highlights important patterns and salary trends in Portugal:

✔ Key Insights

* Minimum wage increased steadily from 2015 to 2022.
* The gender pay gap remains significant and stable. 
* Education is one of the strongest factors influencing salary levels.
* Technology, finance and specialized sectors show the highest salaries.
* Lower salaries are concentrated in traditional services and low-skilled activities.
* The 65+ age group shows higher average salaries, reflecting longer career time and accumulated progression.



🛠️ Tools Used

* Python (ETL)
* Power BI Desktop
* DAX
* Pordata (public data)
* GitHub for version control and documentation



🎯 Skills Developed

* ETL with real-world data
* Cleaning, normalization and standardization of public datasets
* Dimensional modeling
* Creation of professional dashboards
* Analytical storytelling
* Handling incomplete datasets and complex structures



📬 Contact

For suggestions, questions or collaboration:

PC Data Insights – www.pcdatainsights.com



📝 Note

This dashboard was created for educational and portfolio purposes, using public data that may contain natural gaps or inconsistencies.

