# YTD-Sales-Performance-Dashboard_PowerBI
This PowerBI dashboard compares Year-to-Date (YTD) sales performance to the prior year for a company that sells plants. It includes key metrics such as sales, gross profit, and quantity sold compared across 2022-2024.

## Project Overview
This PowerBI dashboard includes the following features:
- **Header Metrics (Cards)**:
  - **YTD**: Current year-to-date sales performance.
  - **PYTD**: Prior year-to-date sales performance.
  - **YTD vs PYTD**: A comparison between YTD and PYTD performance.
  - **Gross Profit**: Gross profit for the current year.
- **Stacked Coulmn Chart**: Displays the YTD performance in stacked columns (with product type within the stacks) vs. a line chart showing the total PYTD performance. The visual can be drilled-up to see the quarterly performance.
- **Treemap**: Displays the top 10 countries with the lowest YTD sales, quantity or gross profit, providing a quick overview of underperforming countries.
- **Waterfall Chart**: Illustrates the YTD vs PYTD performance with drill-down options by country, month, and product type, helping to identify specific areas of lagging performance.
- **Scatter Chart**: Allows customizable slicer values for YTD metrics and gross profit, aiding in the identification of customers who generate high gross profit but require increased sales volume, or vice versa.
- **Dynamic Titles**: Each visual has a dynamic title that automatically updates based on the selected slicer values, enhancing the dashboard's interactivity and user experience.

## Data Source
The data used in this dashboard is contained in a single Excel workbook named `Sales Analysis.xlsx`. The workbook includes the following sheets:
1. **Plant_FACT**: Contains sales data.
2. **Accounts**: The customer master list.
3. **Plant_Hierarchy**: The product master list.
Additionally, a calendar dimensions table was created within PowerBI to facilitate time-based calculations. Multiple relationships (many-to-many and one-to-many) were established between the tables

## Measures and DAX Calculations
All measures and DAX formulas are organized under a dedicated measures table. Key calculations include:
- **PYTD (Prior Year to Date)**: Calculated using the `INPAST` and VAR DAX measures for each slicer value (sales, quantity, and gross profit).
- **YTD (Year to Date)**: Calculated using the `TOTALYTD` DAX measure.

## Target Audience
This dashboard is intended for the top management of the company, especially global sales leaders. It serves as a tool to facilitate discussions with sales leaders in each country, helping the global leader pinpoint which countries are lagging behind and identify specific product types or customers contributing to the performance gap.

**Open in PowerBI**:
   - Open the `Sales Analysis.pbix` file in PowerBI Desktop.

3. **Explore the Dashboard**:
   - Interact with the slicers and select the year to view different metrics and observe how the dynamic titles update accordingly. Also, please use the drill down options for the waterfall and stacked column chart.

