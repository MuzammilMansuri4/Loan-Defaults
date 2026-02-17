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
<img width="658" height="42" alt="p1 dax 5" src="https://github.com/user-attachments/assets/58d59e73-f359-42ad-a302-e5b76d1cdd1d" />
<img width="841" height="94" alt="p1 dax 4" src="https://github.com/user-attachments/assets/d29ca204-4cb7-4b1c-a542-6816ecd7d8a9" />
<img width="689" height="113" alt="p1 dax 3" src="https://github.com/user-attachments/assets/3f912743-b2fa-4532-955f-ba6b8209cc07" />
<img width="731" height="22" alt="p1 dax 2" src="https://github.com/user-attachments/assets/13c9dd56-5c9a-444e-a582-bf3437ca579a" />
<img width="853" height="24" alt="p1 Dax 1" src="https://github.com/user-attachments/assets/6a044210-ea75-4a36-89af-a8d3617f9913" />



### 3. Applicant Demographic and Financial Profile:

* **Report:** https://app.powerbi.com/groups/8c7666de-82f2-4c3c-9f5e-69b2ca6760a6/dashboards/184b2a83-430a-403b-8ee2-77a9fdbac73e?ctid=c48b5cac-8fce-4403-83ff-18f46537aa73&pbi_source=linkShare

<img width="1493" height="827" alt="p2 visual" src="https://github.com/user-attachments/assets/8983cd13-4ea8-4bc7-8fce-76093af2bcc5" />

Overall Demographic of the applicant and their financial Profile can be understood via this report, since default rates in education is high we can further drillthrough on type of education the loan is being taken for where following graph can be seen:

<img width="342" height="268" alt="Education Type" src="https://github.com/user-attachments/assets/4597f9d0-2ace-4800-805f-0b0ad30bf0d3" />

To further analyse, loan amount being given relative to their credit score we can see that high school median loan amount is high but their credit score is either low or very low

<img width="633" height="313" alt="Screenshot 2026-02-18 000128" src="https://github.com/user-attachments/assets/a9bd2564-d9c5-4119-9994-295f4667d357" />

here, decreasing the loan amount being given to these two credit score level could decrease the default rate from education category in future.


* **Following DAX Measures were used in this report:**
<img width="698" height="47" alt="p2 dax5" src="https://github.com/user-attachments/assets/5a3d7af9-d831-4938-b991-d88133f8f405" />
<img width="1284" height="61" alt="p2 dax 4" src="https://github.com/user-attachments/assets/199c2434-bd71-46a0-884f-d3eff51517f4" />
<img width="390" height="51" alt="p2 dax 3" src="https://github.com/user-attachments/assets/2317c6ef-0f1a-4ad4-859a-fc730572a377" />
<img width="487" height="47" alt="p2 dax 2" src="https://github.com/user-attachments/assets/616c3228-6bcd-498c-b87c-5740039881d3" />
<img width="751" height="48" alt="p2 dax 1" src="https://github.com/user-attachments/assets/e8515b2d-d256-4d9f-9899-326a163cd28a" />

### 4. Financial Risk Metrics:
* **Report:** https://app.powerbi.com/groups/8c7666de-82f2-4c3c-9f5e-69b2ca6760a6/dashboards/be9e2237-caca-4713-9132-2b5da9281238?ctid=c48b5cac-8fce-4403-83ff-18f46537aa73&pbi_source=linkShare

<img width="1493" height="786" alt="p3 visual" src="https://github.com/user-attachments/assets/907a5f99-f64a-4185-ac4d-35898edb04af" />

* **Following DAX Measures were used in this report:**
<img width="1225" height="51" alt="p3 dax 3" src="https://github.com/user-attachments/assets/963e16f3-ac1b-4028-bcc1-054cf3031b71" />
<img width="432" height="227" alt="p3 dax 2" src="https://github.com/user-attachments/assets/1b858eed-5294-484b-85b9-341170fb7282" />
<img width="459" height="280" alt="p3 dax 1" src="https://github.com/user-attachments/assets/93e4d0ad-6eee-4be5-b902-c55a6b640657" />



