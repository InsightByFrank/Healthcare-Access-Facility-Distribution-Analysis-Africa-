# 🏥 Healthcare Facility Access & Distribution Intelligence Dashboard

## 📌 Project Title
**Healthcare Access Facility Distribution Analysis (Africa)**

---


![Screenshot 2025-03-21 122548](https://github.com/user-attachments/assets/70e89a0b-04e3-406f-b2b1-a2a7020ebaa7)
![Screenshot 2025-03-21 122617](https://github.com/user-attachments/assets/a57fca20-5644-46d9-9f6d-00ebc499eb49)

## 📖 Description
This project delivers a data-driven Power BI dashboard aimed at examining healthcare facility distribution, funding efficiency, emergency response times, and patient satisfaction across 12 African countries. It explores both rural and urban disparities in healthcare infrastructure, providing strategic insights to government agencies, global health partners, and policy makers.

Through intuitive visualizations and DAX-powered metrics, this report sheds light on the dynamics of funding, population-health resource ratios, and regional needs.

---

## 📂 Table of Content
- [Description](#description)
- [Key Performance Indicators](#key-performance-indicators)
- [Processes](#processes)
- [DAX Measures](#dax-measures)
- [Business Questions Answered](#business-questions-answered)
- [Observations and Data Highlights](#observations-and-data-highlights)
- [Visuals and Analytics Used](#visuals-and-analytics-used)
- [Actionable Insights](#actionable-insights)
- [Expected Outcomes](#expected-outcomes)
- [Conclusion](#conclusion)
- [Contact Me](#contact-me)

---

## 📊 Key Performance Indicators

| KPI                             | Value           |
|----------------------------------|------------------|
| Total Facilities                 | 2,000            |
| Total Funding                    | $231.1 million   |
| Doctor-Patient Ratio             | 540              |
| Avg. Distance to Facility (km)   | 10.6             |
| Avg. Patient Satisfaction (%)    | 77.5%            |
| Facility Distribution (Rural)    | 94%              |
| Facility Distribution (Urban)    | 6%               |
| Avg. Emergency Response Time     | 32.4 minutes     |

---

## ⚙️ Processes

1. **Data Collection & Exploration**  
   - Sourced data from African health facility registries and open datasets.  
   - Focused on 12 countries across Sub-Saharan Africa.

2. **Data Cleaning & Preparation**  
   - Used Power Query for null handling, type conversion, and renaming.  
   - Created structured fact and dimension tables.

3. **Data Modeling**  
   - Defined relationships between regional, funding, facility, and emergency datasets.  
   - Built star schema for scalable modeling.

4. **KPI Design**  
   - Applied DAX to calculate funding ratios, satisfaction metrics, and emergency times.  
   - Created normalized measures for cross-country comparisons.

5. **Dashboard Development**  
   - Designed with user personas: policymakers, health directors, funders.  
   - Implemented slicers, drilldowns, maps, and visual storytelling components.

6. **Testing & Deployment**  
   - Validated DAX results against raw data.  
   - Published report to Power BI Service.

---

## 🧠 DAX Measures

- `Total Funding = SUM('Healthcare Data'[Funding Received (USD)])`
- `Doctor Patient Ratio = DIVIDE(SUM('Healthcare Data'[Population]), SUM('Healthcare Data'[Number of Doctors]))`
- `Funding Per Patient Visit = DIVIDE([Total Funding], SUM('Healthcare Data'[Annual Patient Visits]))`
- `Avg Emergency Response Time = AVERAGE('Healthcare Data'[Emergency Response Time (minutes)])`
- `Region Min-Max Color = IF([Total Facilities] = min_value, "#00A8C6", IF([Total Facilities] = max_value, "#008060", "#D9D9D9"))`

...and several others used to build interactive visualizations.

---

## ❓ Business Questions Answered

1. How is healthcare facility distribution split between urban and rural areas?  
2. Which regions or facility types receive more funding?  
3. Does higher funding correlate with better emergency response?  
4. Which facility types are most cost-efficient?  
5. Where are satisfaction levels highest?

---

## 📌 Observations and Data Highlights

- **Urban vs Rural:** 94% of facilities are rural, but urban gets more funding per facility.  
- **Top Funding Regions:** Southern Zambia ($23M), Western Kenya, Central Malawi.  
- **Response Time:** Rural regions perform slightly better than urban in response times.  
- **Efficiency:** Hospitals are the most cost-effective based on funding per visit.

---

## 📊 Visuals and Analytics Used

- 🌍 **Map Chart** – Facility distribution by region  
- 📊 **Bar Chart** – Funding by region  
- 🍩 **Doughnut Chart** – Patient satisfaction by facility type  
- 🍭 **Lollipop Column** – Response vs Satisfaction by Region  
- 📈 **Scatter Plot** – Funding vs Emergency Response  
- 🎛️ **Slicers/Filters** – Region, Region Type, Facility Type

---

## 🎯 Actionable Insights

1. Prioritize urban zones with high response times for ambulance service investments.  
2. Expand mobile clinics to bridge urban-rural access gaps.  
3. Use performance-based funding to reward high-efficiency facilities.  
4. Focus future investments on high-burden countries like Senegal and Ghana.

---

## 🎯 Expected Outcomes

- 📉 Reduced emergency response times in key regions  
- 😀 Improved patient satisfaction and care delivery  
- 💸 More optimized use of healthcare funding  
- 🧠 Data-backed policy reforms and planning

---

## 🧾 Conclusion

This dashboard highlights critical disparities in healthcare facility distribution and emergency readiness across African countries. It equips stakeholders with powerful insights to implement strategic changes that enhance health equity, funding efficiency, and system-wide responsiveness.

### Live Preview 
[[🔗 Click Here for a walkthrough on my project]](https://app.powerbi.com/groups/me/reports/0f5a0610-f4b9-4c60-89a5-91d877a58852?experience=power-bi)

---

## 📬 Contact Me

**Frank Agba Onwuchekwa**  
📧 Email: Frankgodwin796@gmail.com  
🔗 LinkedIn: [Frank Agba](https://www.linkedin.com/in/frank-agba)  
💬 WhatsApp: +2349168566449
