## Report Overview
This Report focuses on analyzing loan default data to identify patterns, risks, and trends within a financial dataset.
this project demonstrates end-to-end PowerBI workflows from data ingestion via SQL Server to complex DAX modeling and interactive visualization & its analysis.

###  Key Objectives
* **Risk Identification:** Visualize high-risk loan categories to assist in credit decision-making.
* **Temporal Trends:** Analyze how default rates fluctuate over specific time periods.

##  Technical Stack
* **Data Source:** SQL Server Database with which BI DataFlow is connected.
* **ETL Process:** PowerBI Service DataFlows.
* **Dax:** Various Dax Methods applied to facilitate visuals & its analysis.  
* **Visualization:** utilisation of various Graph Types such as time series,categorical etc

### 1. Data Preview:
* **Data Source:** BI service's Dataflow connected to SQL server database that accessess the financial dataset
<img width="791" height="628" alt="DataSource" src="https://github.com/user-attachments/assets/ce1833a1-f6fb-451b-ac07-40b8a0c2d813" />

* **Fields Name & Top rows Details:**
  
  <img width="279" height="391" alt="Field Names" src="https://github.com/user-attachments/assets/8be4dd66-be4b-40ba-94a6-e6eadeca53ae" />
  <img width="2389" height="824" alt="Field Details" src="https://github.com/user-attachments/assets/554a9513-c7bd-4406-904e-012f2f68e00c" />
  
### 2. Loan Default overview:

* **Report:** https://app.powerbi.com/groups/8c7666de-82f2-4c3c-9f5e-69b2ca6760a6/dashboards/0ce5619e-104e-4cae-a32a-6619a4dccb10?ctid=c48b5cac-8fce-4403-83ff-18f46537aa73&pbi_source=linkShare
<img width="1531" height="839" alt="p1 visual" src="https://github.com/user-attachments/assets/eb557912-c950-4f95-a767-59ae92b4d9c6" />
during the year 2016 & 2014 where we see 0.25% increase in defaults

 * **Drillthrough reveals the changes in loan amount given by purpose sees a shift from 2014 to 2016 is home loan to education loan being the top contributor:**
  
  * **2014:**<img width="1493" height="814" alt="2014 sqaure" src="https://github.com/user-attachments/assets/2bd0ddfd-0129-48d1-93d3-fd0f99953369" />

  * **2016:**<img width="1495" height="817" alt="2016 sq" src="https://github.com/user-attachments/assets/463fbe00-782d-4ac3-9591-fd1006049438" />

to further validate the data keeping the 2016 filter on, Education loan does become the top contributor in default as well while home loan being least likely to default in both the cases,  since from 2016 loan distribution towards the education sector has increased the rise in default rate can be seen.

<img width="628" height="455" alt="purpose 2016" src="https://github.com/user-attachments/assets/647b7a04-ac15-4ea6-992f-85add5a1bd86" />


* **Following DAX Measures were used in this report:**
1.
<img width="658" height="42" alt="p1 dax 5" src="https://github.com/user-attachments/assets/58d59e73-f359-42ad-a302-e5b76d1cdd1d" />

2.
  <img width="841" height="94" alt="p1 dax 4" src="https://github.com/user-attachments/assets/d29ca204-4cb7-4b1c-a542-6816ecd7d8a9" />

3.
  <img width="689" height="113" alt="p1 dax 3" src="https://github.com/user-attachments/assets/3f912743-b2fa-4532-955f-ba6b8209cc07" />

4.
  <img width="731" height="22" alt="p1 dax 2" src="https://github.com/user-attachments/assets/13c9dd56-5c9a-444e-a582-bf3437ca579a" />

5.
  <img width="853" height="24" alt="p1 Dax 1" src="https://github.com/user-attachments/assets/6a044210-ea75-4a36-89af-a8d3617f9913" />



### 2. Applicant Demographic and Financial Profile:

Report: https://app.powerbi.com/groups/8c7666de-82f2-4c3c-9f5e-69b2ca6760a6/dashboards/184b2a83-430a-403b-8ee2-77a9fdbac73e?ctid=c48b5cac-8fce-4403-83ff-18f46537aa73&pbi_source=linkShare

<img width="1493" height="827" alt="p2 visual" src="https://github.com/user-attachments/assets/8983cd13-4ea8-4bc7-8fce-76093af2bcc5" />

Overall Demographic of the applicant and their financial Profile can be understood via this report, since default rates in education is high we can further drillthrough on type of education the loan is being taken for where following graph can be seen:

<img width="342" height="268" alt="Education Type" src="https://github.com/user-attachments/assets/4597f9d0-2ace-4800-805f-0b0ad30bf0d3" />






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

