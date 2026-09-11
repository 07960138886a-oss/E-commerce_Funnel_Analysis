<h1 align="center">E-commerce Funnel Analysis</h1>

1. Project Introduction                 
An end-to-end e-commerce funnel analytics project that uses Python to analyze Amazon user behavior data, track stage-to-stage session drop-offs, analyze multi-dimensional drop-off drivers, and deliver strategic recommendations to boost conversion rates and sales.

2. Executive Summary & Key Metrics
Analytic overview across a customer interaction base of 10,000 sessions (21,676 event records) during 2026-07-15 to 2026-08-14:              
(1) Key Metrics:                      
1,063 Total Orders | 10.63% Overall Conversion Rate | $1,198,361.56 Total Revenue | $1,127.34 Average Order Value (AOV).        
(2) Primary Funnel Bottlenecks:       
The Purchases stage experienced the highest drop-off rate (69.76% drop-off from Basket Adds to Purchases overall), representing significant cart abandonment across the user journey.
 <img width="1043" height="421" alt="截屏2026-09-06 00 41 33" src="https://github.com/user-attachments/assets/070e23db-eed2-4747-a522-b951effd1b5c" />.       
This pattern also occurs across each segmented dimension (channels, devices, regions, and product categories).        
(3) Performance Highlights:       
    <table border="0">
  <tr>
    <td align="center" width="33%">
      <b>Organic Search</b><br>
      <sub>Top Marketing Channel (11.18% CVR)</sub>
    </td>
    <td align="center" width="33%">
      <b>Appliances</b><br>
      <sub>Best Product Category (11.40% CVR)</sub>
    </td>
    <td align="center" width="33%">
      <b>Wales</b><br>
      <sub>Leading Regional Market (11.39% CVR)</sub>
    </td>
  </tr>
  <tr>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/2aaef3da-5cc2-47a3-a2b5-2c7917215513" width="100%"/>
    </td>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/170e391f-889f-4f6b-a1f5-d646231b214d" width="100%" />
    </td>
    <td align="center" valign="top">
      <img src="https://github.com/user-attachments/assets/b2ec0d63-0479-4b83-aa8a-abb5b65512cd"  width="100%" />
    </td>
  </tr>
</table>           




        
3\. Pipeline Architecture & Tech Stack           
[ Raw Data Generation ] ──> [ Session Aggregation (Pandas) ] ──> [ Funnel & KPI Modeling ] ──> [ Multi-Dimensional Analysis ] ──> [ Interactive Visualization & Insights ]             
(1) Data Preparation & Data Cleaning: Python (Pandas, Numpy, Datetime)                 
(2) Behavioral & Funnel Analytics: Python (Pandas, Aggregation, Time-series modeling)               
(3) Data Visualization: Python (Matplotlib, Seaborn, Plotly), Power BI.                  

4\. User Funnel Performance Dashboards & Drop-off Diagnostics               
<table border="0" width="100%">
  <tr>
    <td align="center" width="50%"><b>(1) User Funnel Performance Dashboard</b></td>
    <td align="center" width="50%"><b>(2) Funnel Drop-off Diagnostics</b></td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/99e64e24-9aed-4f8d-ba50-a06189971b7f" style="width:100%;" />
    </td>
    <td align="center" width="50%">
      <img src="https://github.com/user-attachments/assets/f72c2a22-5d76-4d8a-8249-c7d9a9c18ae8" style="width:100%;" />
    </td>
  </tr>
</table>
<a href="./1funnel%20analysis.pbix">Click here to download the interactive Power BI report (.pbix)</a>.          
 

5\. Python Code & Analytical Implementation           
(1) Synthetic Data Generation & Data Cleaning         
Generated 10,000 user session records using Faker with custom event conditional probabilities.       
Data quality checks, timestamp transformations, and duration calculations were executed seamlessly.       
View simulated raw dataset: [amazon_funnel_analysis_data.csv](./amazon_funnel_analysis_data.csv).       
(2) Session-Level Aggregation & Multi-Dimensional EDA         
Aggregated raw event logs into session-level records (`session_summary`) to evaluate conversion rates, drop-off rates, and Revenue per Session (RPS) across channels, devices, product categories, regions, and time periods.        
View the full analysis & Python implementation and outputs: [Amazon_Funnel_Analysis.ipynb](./Amazon_Funnel_Analysis.ipynb)

6\. Strategic Recommendations       
(1) Cart Abandonment Recovery: Address the 69.76% drop-off at the Purchases stage by streamlining checkout UX and launching automated cart abandonment email campaigns, unlocking an estimated $2,766,724.01 in potential revenue recovery.       
(2) Budget Optimization: Reallocate marketing spend toward high-ROI channels, prioritizing Organic Search (11.18% CVR) and Sponsored Products(10.61% CVR).       
(3) Regional Strategy Replication: Benchmark and replicate successful promotional strategies from Wales (11.39% CVR) across lower-performing markets such as North Ireland (9.84% CVR).        
(4) Category Promotion: Increase homepage visibility and ad placements for top-converting categories like Appliances (11.40% CVR) and Bedding (10.82% CVR).           
