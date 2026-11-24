05_DASHBOARD - CUSTOMER VOICE RADAR (Power BI)

1. CustomerVoiceRadar.pbip  (+ CustomerVoiceRadar.Report and CustomerVoiceRadar.SemanticModel folders)
   Power BI project: open CustomerVoiceRadar.pbip in Power BI Desktop (keep the 3 items together),
   click Refresh if asked. Interactive dashboard, 5 pages:
   1) Overview  2) Voice of Customer  3) Root Cause  4) Early Warning  5) Data Quality
   Slicers (year, sales channel, city) are synced across pages.

2. Dashboard_Data.xlsx
   The data model used by the dashboard (FactOrders, FactReviews, ReviewTopics,
   DimCustomer with health score, DimDate, Anomalies, DataQuality, CleaningLog).
   Built from: 01_Data_Engineering (Cleaned_Data), 03_Text_Analysis
   (07_Reviews_Analyzed.csv) and 04_Insights_Recommendations (Task 4).

3. CustomerVoiceRadar_Theme.json
   Power BI color theme of the project.

Fonts: titles use Amiri (install from Font_Amiri if titles look different);
numbers use Segoe UI.

Definitions: late delivery = more than 6 days; complaint = rating <= 2;
sales = line_revenue after discount (cleaned data).
