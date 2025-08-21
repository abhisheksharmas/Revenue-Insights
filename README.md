# 📊 Revenue Insights in the Hospitality Domain

*An interactive Power BI dashboard providing deep insights into the revenue and performance of Atliq Hotels across India.*

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-Analysis%20Expressions-blue)](https://learn.microsoft.com/en-us/dax/)


---

![Dashboard Overview](Revenue%Insights/ss1.png)

---

### 🎯 Problem Statement

The hospitality industry relies on data-driven decisions to optimize pricing, manage occupancy, and maximize revenue. Atliq Hotels, a major hotel chain, needed a centralized and interactive way to track key business metrics across their various properties. The goal of this project was to develop a comprehensive Power BI dashboard that provides insights into:

-   Revenue trends and performance.
-   Occupancy rates and booking patterns.
-   Average Daily Rate (ADR) and Revenue Per Available Room (RevPAR).
-   Performance by city, property, and room class.

This dashboard empowers stakeholders to identify top-performing properties, understand customer behavior, and make strategic decisions to enhance profitability.

---

### 📸 Project Snapshots

Here are a few snapshots of the main dashboard views:

**Dashboard - Main View:** Provides a high-level overview of all key metrics, with filters for date range, city, and hotel property.
![Dashboard - Main View](Revenue%Insights/ss1.png)

**Dashboard - Details View:** Offers a more granular look at performance by room type, booking platform, and booking status.
![Dashboard - Details View](Revenue%Insights/ss2.png)

---

### 📈 Key Performance Indicators (KPIs)

The dashboard tracks several critical metrics, derived from the data using DAX:

-   **Total Revenue:** The total revenue realized from all successful bookings.
-   **Total Bookings:** The total number of unique bookings made.
-   **Occupancy %:** The percentage of available rooms that were successfully booked.
    -   $Occupancy \% = \frac{\text{Total Successful Bookings}}{\text{Total Capacity}}$
-   **Average Daily Rate (ADR):** The average revenue earned per occupied room per day.
    -   $ADR = \frac{\text{Total Revenue}}{\text{Total Successful Bookings}}$
-   **Revenue Per Available Room (RevPAR):** A key metric that measures a hotel's ability to fill its available rooms at an average rate.
    -   $RevPAR = ADR \times Occupancy \%$
-   **Realisation %:** The percentage of revenue generated from confirmed bookings that was actually realized.
-   **Week-over-Week (WoW) Change %:** Dynamic calculation of the percentage change in key metrics compared to the previous week.

---

### 🛠️ Technologies Used

-   **Power BI Desktop:** The core tool for data modeling, DAX calculations, and dashboard creation.
-   **DAX (Data Analysis Expressions):** Used to create powerful and flexible calculations.
-   **Power Query:** For data extraction, transformation, and loading (ETL).
-   **Microsoft Excel:** Used initially to inspect the data and review the metrics list.

---
