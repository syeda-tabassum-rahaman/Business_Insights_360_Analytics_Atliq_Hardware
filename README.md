# AtliQ Hardware: Business Insights 360

**[Live Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiYjc0ZDVhM2YtOGEwNS00MDZmLWEwMTAtZDQ0MmRmYmY5MDkxIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)**

*(<img width="866" height="557" alt="Home" src="https://github.com/user-attachments/assets/180e371c-7cea-4dad-a910-8c0ccd221e4b" />)*

## 📌 Project Overview & Business Value

**The Challenge:** AtliQ Hardware, a global vendor of computer hardware and peripherals, faced unexpected losses after expanding into the American market. Leadership identified the root cause: a heavy reliance on outdated, static Excel spreadsheets for data analysis, putting them at a severe disadvantage against competitors with robust analytics teams.

**The Solution:** To transition the company to data-driven decision-making, this project delivers an end-to-end, enterprise-level Power BI solution. Processing over 1.8 million transaction records from MySQL and Excel, the "Business Insights 360" dashboard replaces manual reporting with an automated, centralized tool. It equips Finance, Sales, Marketing, Supply Chain, and Executive stakeholders with immediate visibility into critical KPIs, performance against benchmarks, and actionable historical trends.

## 💡 Key Business Solutions Provided
By transitioning from static Excel sheets to an interactive Power BI environment, this solution empowers AtliQ Hardware to directly address its core operational challenges:

* **Automated Financial Tracking:** Replaced manual P&L generation with dynamic tracking of Net Sales, Gross Margin, and Net Profit against Last Year (LY) and Target benchmarks.
* **Inventory Risk Mitigation:** Developed a custom Supply Chain view to calculate Forecast Accuracy and Net Error, instantly flagging products at risk of **Excess Inventory (EI)** or **Out of Stock (OOS)**.
* **Granular Profitability Analysis:** Enabled drill-downs into Unit Economics and Gross Margin variances, allowing stakeholders to identify the exact customers, regions, or products causing financial losses.
* **Executive Visibility:** Centralized market share trends and revenue contributions, providing the C-suite with immediate clarity on their American expansion and overall global performance.

## 🛠️ Tech Stack & Methodologies
* **BI Tool:** Microsoft Power BI Desktop & Service
* **Data Sources:** MySQL Database (1.8M+ records), Excel/CSV files
* **ETL & Data Prep:** Power Query (Data cleaning, dynamic date tables, reducing dataset size for performance)
* **Data Modeling:** Snowflake Schema integrating 11 Fact and Dimension tables
* **Analytics:** Advanced DAX (Time Intelligence, dynamic benchmarking, custom tooltips)
* **UI/UX Design:** Page navigation, bookmarks, and dynamic parameter slicers

## 📊 Dashboard Structure
The report is strategically divided into six functional views to provide targeted insights for different business units:

* **Home:** Centralized navigation hub with dynamic data-refresh indicators.
* **Finance View:** Detailed P&L (Profit & Loss) analysis, Net Sales vs. Target benchmarks, and Gross Margin tracking over time.
* **Sales View:** Customer performance analysis, unit economics, and revenue drivers across various channels.
* **Marketing View:** Product and segment profitability, highlighting Net Profit % variance across regions.
* **Supply Chain View:** Forecast accuracy tracking and inventory risk management (identifying Excess Inventory vs. Out of Stock risks).
* **Executive View:** Consolidated high-level KPIs, market share trends, and top customer/product insights for C-level leadership.

## 🗄️ Dataset & Data Architecture

### The Dataset
The project processes approximately 1.8 million records across 11 tables, integrating fragmented data into a unified single source of truth:
* **MySQL Databases:** Contains core dimensional data (customers, markets, products) and massive transactional fact tables (monthly sales, monthly forecasts, and invoice deductions).
* **Excel Files:** Supplementary business data including FY targets, operational expenses, and market share statistics.

### The Data Model
A robust **Snowflake Schema** was designed to optimize performance and accurately map complex business entities. 

* **Core Structure:** Centralized Fact tables (Sales, Forecasts, Actuals) are connected to surrounding Dimension tables (Custom Fiscal Date, Customer, Product, Market).
* **Performance Optimization:** Heavy data transformations and denormalization were handled upstream in Power Query. Redundant DAX calculated columns were intentionally minimized in the front-end to keep the file size lean and the dashboard highly responsive.

*(<img width="725" height="788" alt="data model" src="https://github.com/user-attachments/assets/efac6507-1fb2-440f-97a8-5302257b932a" />)*

## 🎯 Conclusion & Business Impact
The "Business Insights 360" project successfully transforms AtliQ Hardware's analytical capabilities from reactive to proactive. The company is no longer operating in the dark or relying on fragmented spreadsheets. By consolidating millions of rows of data into a single, highly responsive dashboard, leadership can now confidently pinpoint loss-making areas, optimize supply chain forecasting, and make data-driven decisions to regain their competitive edge in the market.
