# Coffee-Sales-Analysis
Analysing the sales of different coffee variants helps us understand consumer preferences.

## Overview

This project provides an **end-to-end data analytics solution** for coffee sales data, leveraging advanced Excel features to deliver actionable insights through a dynamic, interactive dashboard. It involved gathering raw data from disparate tables, performing extensive data cleaning and transformation, and building a visually appealing dashboard optimized for easy manipulation and interpretation, demonstrating proficiency in data manipulation, data modeling principles (including the use of lookup functions), data validation, and professional business intelligence visualization in Excel.


## Dataset

The analysis utilizes a comprehensive dataset concerning coffee bean sales. The raw data was structured across three main tables:

*   **Orders Table:** Contains transactional details including `Order ID`, `Order Date`, `Customer ID`, `Product ID`, and `Quantity` sold.
*   **Customers Table:** Contains customer information, including `Customer ID` (the primary key), `Customer Name`, `Email`, geographic location (City, Country), and `Loyalty Card` status.
*   **Products Table:** Contains product specifications, including `Product ID` (the primary key), `Coffee Type`, `Roast Type`, `Size`, `Unit Price`, and `Profit` associated with the product.

Key characteristics of the sales data include:

*   **Coffee Types:** Four variants are sold: **Arabica**, **Excelsa**, **Liberica**, and **Robusta**.
*   **Roast Types:** Coffees are categorized by roast: **Dark**, **Light**, and **Medium**.
*   **Package Sizes:** Coffee beans are sold in specific weights: **0.2 kg**, **0.5 kg**, **1.0 kg**, and **2.5 kg** packages.
*   **Sales Regions:** Products are sold in three countries: the **U.S.**, **Ireland**, and the **UK**.

## Tools

*   **Microsoft Excel:** Utilized for all stages of the project, including data modeling, data cleaning, analysis, and dashboard creation.
*   **Excel Functions:** Advanced formulas employed for data lookup and transformation, specifically **XLOOKUP** and the dynamic combination of **INDEX MATCH**.
*   **Pivot Tables and Pivot Charts:** Used for summarizing data and creating core visualizations.
*   **Slicers and Timelines:** Implemented to provide interactive, dynamic filtering capabilities for the end-user.

## Steps

1.  **Data Gathering and Merging (Lookups):**
    *   Missing customer information (Name, Email, Country, Loyalty Card status) and product details (Coffee Type, Roast Type, Size, Unit Price) were appended to the Orders table by performing lookups against the Customers and Products tables.
    *   **XLOOKUP** was used for basic information lookup, including implementing **IF function logic** to handle and replace missing values (represented as zeros) in the email column with blanks.
    *   A **dynamic INDEX MATCH** function was employed to efficiently pull multiple product attributes (coffee type, roast type, size, and price) with a single formula, showcasing dynamic referencing skills.

2.  **Data Cleaning and Transformation:**
    *   A new **Sales** column was calculated by multiplying the `Unit Price` by the `Quantity Sold`.
    *   Abbreviated codes for `Coffee Type` (e.g., ROB, ARA) and `Roast Type` (e.g., M, L, D) were converted into their full, user-friendly names (e.g., Robusta, Medium) using multiple **IF functions**.
    *   Data formatting standards were applied: `Order Date` was standardized (e.g., 05-Sep-2019), product `Size` was appended with the "kg" metric, and `Unit Price` and `Sales` were formatted to **US Dollars** currency.
    *   The entire cleaned data range was converted into a named **Excel Table ("Orders Table")** to ensure all future analyses (Pivot Tables) dynamically incorporate new data or columns automatically upon refresh.

3.  **Analysis and Visualization:**
    *   Pivot Tables were created to summarize key metrics necessary for the visualization components.
    *   Three primary charts were developed: Total Sales Over Time, Sales By Country, and Top 5 Customers.

4.  **Dashboard Finalization:**
    *   **Timeline and Slicers** were added to the dashboard. Slicers included **Roast Type Name**, **Size**, and **Loyalty Card** status.
    *   All interactive elements (Timeline and Slicers) were connected to **all three pivot charts** to ensure cross-filtering functionality across the entire dashboard.
    *   The final dashboard interface was customized for a clean, professional aesthetic by adjusting backgrounds, font colors, and hiding unnecessary grid lines and scrollbars.
  
  ## Dashboard

The resulting interactive dashboard provides a single, high-level view of coffee sales performance, with comprehensive segmentation filters.

**Key Visualizations:**

| Visualization | Type | Purpose |
| :--- | :--- | :--- |
| **Total Sales Over Time** | Line Chart | Tracks sales trends across the entire dataset, segmented by the four `Coffee Type` names (Arabica, Excelsa, Liberica, Robusta). |
| **Sales By Country** | Bar Chart | Shows total sales volume distributed across the three major sales regions (U.S., Ireland, UK). |
| **Top 5 Customers** | Bar Chart | Highlights the five highest-performing customers based on their total sales. |

**Interactive Filters:**

The dashboard includes dynamic controls to segment the data instantly:

*   **Timeline:** Filters data based on the `Order Date`.
*   **Roast Type Name Slicer:** Allows selection of Dark, Light, or Medium roasts.
*   **Size Slicer:** Filters by package size (0.2 kg, 0.5 kg, 1.0 kg, 2.5 kg).
*   **Loyalty Card Slicer:** Filters sales based on whether customers possess a loyalty card (Yes/No).

## Results

Analysis of the comprehensive sales dashboard revealed crucial performance metrics:

*   **Geographic Performance:** The largest portion of total sales originates from the **United States** at **$35,639**. Sales in Ireland totaled **$6,697**, and the United Kingdom accounted for **$2,799**.
*   **Top Customer Segmentation:** The top performing customer by sum of sales is **Allis Wilmore** ($317), followed closely by **Brenn Dundredge** ($307), **Terri Farra** ($289), **Nealson Cuttler** ($282), and **Don Flintiff** ($278).






