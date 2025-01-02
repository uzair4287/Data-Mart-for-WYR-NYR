# NYR & WYR Data Mart for Bed Occupency

## Overview

This project demonstrates my technical expertise and problem-solving skills in designing and implementing a Data Mart for Bed Occupancy Analysis across care centers in North Yorkshire (NYR) and West Yorkshire (WYR). Using SQL Server Integration Services (SSIS), I built an efficient ETL pipeline to consolidate data from the separate databases of NYR and WYR into a unified structure.

The project highlights my ability to:

- Work with real-world data challenges, such as merging disparate databases.
- Implement advanced ETL concepts, including incremental loading and Slowly Changing Dimensions (SCD).
- Build a scalable and maintainable data mart that supports robust reporting and analysis.
- The centralized data mart provides insights into Bed Occupancy Rates, a key metric for evaluating resource utilization across care centers.
- This project not only showcases my technical skills but also my ability to solve operational challenges using data engineering best practices.



## Introduction
Healthcare organizations in North Yorkshire and West Yorkshire maintain separate databases for their care facilities, creating challenges in:

- Aggregating and analyzing data across regions.
- Gaining a unified view of bed occupancy rates to optimize resource allocation.

To address these issues, I designed and implemented a Data Mart using SSIS, incorporating key data engineering concepts like:

1. Incremental Loading: Ensuring efficient data updates by only processing new or changed records.
2. Slowly Changing Dimensions (SCD): Managing historical changes in dimension data (e.g., facility capacity updates) to maintain accuracy in reporting.
3. Data Transformation: Standardizing and cleaning data to ensure consistency across multiple sources.

By completing this project, I have demonstrated my proficiency in:

- Building robust ETL pipelines.
- Handling complex data integration tasks.
- Using SSIS and SQL to create solutions that drive actionable insights.

The resulting data mart serves as a foundation for unified reporting and provides decision-makers with a clear picture of bed utilization across the regions' care centers.

## Skills Demonstrated

### Data Mart and Star Schema Design

Overview: Designed a star schema to optimize reporting and analytical performance.
Schema Components:
Fact Table: Stored aggregated data related to bed occupancy, including counts and occupancy rates.
Dimension Tables: Captured descriptive attributes of care centers, bed types, and time periods.
Star Schema Benefits:
Simplified queries for KPI generation.
Improved performance for large-scale reporting.
Result: Built a well-structured data mart supporting efficient analysis and scalability.

 KPI Analysis and Selection

Initial KPI Exploration:
Duration of Bed Allocation: Investigated but required additional data on patient assignments.
Duration of Bed Occupancy: Explored but data limitations prevented meaningful insights.
Final KPI Selected:
Bed Occupancy Rate: Chosen as the primary metric due to its relevance and available data.
Formula: 
Bed Occupancy Rate
=
Occupied Beds
Total Beds Available
×
100
Bed Occupancy Rate= 
Total Beds Available
Occupied Beds
​
 ×100.
Rationale:
Focused on a KPI that could be reliably calculated and provide actionable insights.
Demonstrated adaptability and critical thinking in data analysis.

01 Loading into staging data flow

<img width="260" alt="01 Loading into staging data flow" src="https://github.com/user-attachments/assets/818be6d7-86eb-46ee-80c9-e757c5ef7409">

02 Loading in to staging
<img width="577" alt="02 Loading in to staging" src="https://github.com/user-attachments/assets/69a7b54c-d314-4b2f-bcf2-f915a14a6026">

03 pakage stage to dm

<img width="197" alt="03 pakage stage to dm" src="https://github.com/user-attachments/assets/f9c47f31-abae-4763-8e38-49b875b0359a">

04 loding in dimesnion

<img width="366" alt="04 loding in dimesnion" src="https://github.com/user-attachments/assets/2a72c646-9d6c-4982-8a4b-91c243106243">

05 loading into fact

<img width="270" alt="05 loading into fact" src="https://github.com/user-attachments/assets/7e27df3d-a1d3-4ef0-b0de-e0be1c021943">

