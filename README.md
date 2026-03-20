# ⚓ Marine Accident Analysis Dashboard (India 2023)

--

## 🧠 Project Overview

This project provides a comprehensive analysis of marine accidents occurring in Indian waters during 2023. Using Power BI and DAX, the dashboard transforms raw accident logs into strategic insights regarding maritime safety, vessel vulnerability, and regional risk hotspots.

The goal is to identify patterns in maritime mishaps to support better safety protocols and resource allocation for rescue operations.

--

## ❓ Business / Analytical Questions


Which vessel types (e.g., Tugs, Fishing Boats) are most prone to accidents?

What are the deadliest accident types based on fatality rates?

Is there a seasonal trend or specific months with higher accident frequencies?

Which locations (ports/coasts) require enhanced maritime surveillance?

What percentage of accidents result in a total vessel loss?

--

## 📁 Dataset Information
Source: Marine Accident Records (India, 2023)

Key Features: Vessel Type, Accident Type (Sinking, Fire, etc.), Location, Fatalities, Injuries, and Outcome.

Size: 186 recorded incidents across major Indian maritime hubs.

--

## 📊 Dashboard Features
KPI Tiles: Instant view of Total Accidents, Deaths, and Injuries.

Risk Metrics: Custom measures for "Death Rate per Accident" and "% Vessel Loss".

Time Intelligence: Rolling 3-month average to identify pollution/accident spikes.

Geospatial Analysis: Mapping of accidents across locations like Kolkata, Goa, and Chennai.

Interactive Slicers: Filter data by Vessel Type, Location, or Outcome.

--

## 🖼️ Dashboard Preview

.

--

## 🔍 Key Insights

High-Risk Vessels: Specific vessel types like Tugs and Dredgers show a higher frequency of "Vessel Lost" outcomes.

Severity Hotspots: While some locations have more accidents, others have a higher Death Rate, indicating more severe incidents in those regions.

Temporal Trends: The rolling average reveals specific months where maritime risks peak, potentially linked to monsoon seasons.

--

## 💡 Recommendations

Safety Audits: Prioritize safety inspections for vessel types with the highest accident-to-loss ratio.

Regional Training: Focus rescue and safety training in locations identified as high-severity zones.

Predictive Monitoring: Use the rolling average trends to increase maritime patrolling during high-risk months.

--

## 🤖 Analytical Measures (DAX)

This project utilizes advanced DAX to drive insights:

Rolling 3-Month Average: AVERAGEX(DATESINPERIOD(...), [Total Accidents], -3, MONTH)

Vessel Loss %: DIVIDE(COUNTROWS(FILTER(Table, [Outcome]="Vessel lost")), [Total Accidents])

Fatality Rate: Logical division of total deaths by total incident count per category.

--

## 🛠️ Tools & Technologies Used

Power BI Desktop: Dashboard creation and Data Modeling.

DAX (Data Analysis Expressions): For complex calculated measures.

Power Query: Data cleaning and transformation.

Excel/CSV: Data source.

--

## 🚀 How to View the Project

Download the .pbix file from the Dashboard/ folder.

Open it using Power BI Desktop.

If the data links are broken, point the data source to the marine_accidents_india_2023.csv file in the Data/ folder.

--

## 🙌 Author

Sanchit G. Barne

--
