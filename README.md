## Report Overview
This Report focuses on analyzing loan default data to identify patterns, risks, and trends within a financial dataset.
this project demonstrates end-to-end PowerBI workflows from data ingestion via SQL Server to complex DAX modeling and interactive visualization & its analysis.

### 🎯 Key Objectives
* **Risk Identification:** Visualize high-risk loan categories to assist in credit decision-making.
* **Temporal Trends:** Analyze how default rates fluctuate over specific time periods (timestamps)

## 🛠️ Technical Stack
* **Data Source:** SQL Server Database with which BI DataFlow is connected.
* **ETL Process:** PowerBI Service DataFlows.
* **Dax:** Various Dax Methods applied to facilitate visuals & its analysis.  
* **Visualization:** utilisation of various Graph Types such as time series,categorical etc

### 1. Data Preview:
* **Data Source:** BI service's Dataflow connected to SQL server database that accessess the financial dataset
<img width="791" height="628" alt="DataSource" src="https://github.com/user-attachments/assets/ce1833a1-f6fb-451b-ac07-40b8a0c2d813" />

* **Fields Names & Top rows Details:**
  
  <img width="279" height="391" alt="Field Names" src="https://github.com/user-attachments/assets/8be4dd66-be4b-40ba-94a6-e6eadeca53ae" />
  <img width="2389" height="824" alt="Field Details" src="https://github.com/user-attachments/assets/554a9513-c7bd-4406-904e-012f2f68e00c" />
  
### 2. 

The core report page provides a comprehensive look at the loan portfolio. It features time-series analysis and categorical breakdowns.
![Dashboard Overview](YOUR_LINK_HERE_1)



To ensure transparency, the report includes a dedicated section for viewing raw field names and specific data details, ensuring the underlying SQL data is correctly mapped.
![Data Preview](YOUR_LINK_HERE_2)

### 3. DAX & Business Logic
This project utilizes several custom DAX measures to calculate metrics like "Year-to-Date Defaults" and "Average Loan Risk."
![DAX Code Sample](YOUR_LINK_HERE_3)

## 💡 Key Insights
* **Trend Analysis:** Identified specific months with higher default spikes using timestamped data.
* **Portfolio Health:** Segmented the data to show which loan types contribute most to the overall risk profile.

## 🚀 How to Run the Project
1. Clone this repository.
2. Ensure you have Power BI Desktop installed.
3. Open the `.pbix` file (Note: As the data is connected to a private SQL Server via DataFlow, visuals may require a local data refresh or dummy dataset to populate).

