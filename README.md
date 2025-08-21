# 📊 Revenue Insights in the Hospitality Domain

*An interactive Power BI dashboard providing deep insights into the revenue and performance of Atliq Hotels across India.*

[![Power BI](https://img.shields.io/badge/Power%20BI-Desktop-yellow)](https://powerbi.microsoft.com/)
[![DAX](https://img.shields.io/badge/DAX-Analysis%20Expressions-blue)](https://learn.microsoft.com/en-us/dax/)
[![SQL](https://img.shields.io/badge/SQL-Data%20Cleaning-lightgrey)](https://www.mysql.com/)

---

![Dashboard Overview](ss1.png)

### 📖 Table of Contents
* [Problem Statement](#-problem-statement)
* [Live Dashboard](#-live-dashboard)
* [Project Snapshots](#-project-snapshots)
* [Key Performance Indicators (KPIs)](#-key-performance-indicators-kpis)
* [Data Model](#-data-model)
* [Project Workflow](#-project-workflow)
* [Technologies Used](#-technologies-used)
* [How to Use This Project](#-how-to-use-this-project)
* [Contact](#-contact)

---

### 🎯 Problem Statement

The hospitality industry relies on data-driven decisions to optimize pricing, manage occupancy, and maximize revenue. Atliq Hotels, a major hotel chain, needed a centralized and interactive way to track key business metrics across their various properties. The goal of this project was to develop a comprehensive Power BI dashboard that provides insights into:

-   Revenue trends and performance.
-   Occupancy rates and booking patterns.
-   Average Daily Rate (ADR) and Revenue Per Available Room (RevPAR).
-   Performance by city, property, and room class.

This dashboard empowers stakeholders to identify top-performing properties, understand customer behavior, and make strategic decisions to enhance profitability.

---

### 🔗 Live Dashboard

A live, interactive version of the dashboard can be accessed here:

➡️ **[View the Live Power BI Report](https://app.powerbi.com/view?r=eyJrIjoiYOUR_REPORT_ID_HEREIiwidCI6I...)** *(Note: Please replace the link above with your actual public Power BI report link.)*

---

### 📸 Project Snapshots

Here are a few snapshots of the main dashboard views:

**Dashboard - Main View:** Provides a high-level overview of all key metrics, with filters for date range, city, and hotel property.
![Dashboard - Main View](ss1.png)

**Dashboard - Details View:** Offers a more granular look at performance by room type, booking platform, and booking status.
![Dashboard - Details View](ss2.png)

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

### 🗂️ Data Model

The project uses a clean and efficient **Star Schema** data model within Power BI to ensure fast and accurate reporting.

-   **Fact Tables:**
    -   `fact_bookings`: Contains transactional data for each individual booking.
    -   `fact_aggregated_bookings`: A summary table with daily aggregated booking counts and capacity.
-   **Dimension Tables:**
    -   `dim_date`: Provides date-related attributes like week number and day type.
    -   `dim_hotels`: Contains details for each hotel property, including name, category, and city.
    -   `dim_rooms`: Defines the different room classes (Standard, Elite, etc.).

This structure allows for easy slicing and dicing of the data across multiple dimensions.

---

### 🚀 Project Workflow

1.  **Data Loading and Cleaning:** Imported the five CSV files into Power BI. Performed initial data cleaning and transformation using Power Query to handle null values and ensure data type consistency.
2.  **Data Modeling:** Established relationships between the fact and dimension tables to create the star schema.
3.  **DAX Measures & Calculated Columns:** Created over 25 DAX measures to calculate the KPIs listed above, including complex time-intelligence functions for WoW analysis.
4.  **Dashboard Design & Visualization:** Designed an intuitive and visually appealing dashboard with a logical layout, using various charts, cards, slicers, and bookmarks to enhance user experience.
5.  **Validation:** Cross-validated the dashboard numbers with the raw data and stakeholder requirements to ensure accuracy.

---

### 🛠️ Technologies Used

-   **Power BI Desktop:** The core tool for data modeling, DAX calculations, and dashboard creation.
-   **DAX (Data Analysis Expressions):** Used to create powerful and flexible calculations.
-   **Power Query:** For data extraction, transformation, and loading (ETL).
-   **Microsoft Excel:** Used initially to inspect the data and review the metrics list.

---

### ⚙️ How to Use This Project

To explore the dashboard on your local machine:

1.  **Download Power BI Desktop:** Make sure you have the latest version of [Power BI Desktop](https://powerbi.microsoft.com/en-us/downloads/) installed.
2.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/revenue-insights-hospitality.git](https://github.com/your-username/revenue-insights-hospitality.git)
    cd revenue-insights-hospitality
    ```
3.  **Open the `.pbix` file:** Launch Power BI Desktop and open the `Revenue Insights in the Hospitality Domain.pbix` file. The dashboard and all underlying data will be loaded.

---

### 📬 Contact
Your Name – [your.email@example.com](mailto:your.email@example.com)

LinkedIn: [https://linkedin.com/in/your-linkedin-profile](https://linkedin.com/in/your-linkedin-profile)

Project Link: [https://github.com/your-username/revenue-insights-hospitality](https://github.com/your-username/revenue-insights-hospitality)
