# Power_BI_Star_Schema_Webshop
A Power BI project, using artificial webshop data to create a star schema model and report.

## Quick Links
- Artificial Webshop Dataset: [Artifical Webshop Dataset](artificial_webshop_data.xlsx)
- Power BI project file: [Project File](Webshop_star_schema_project.pbix)
- Other projects I have made: [Portfolio Website](https://lucashoffschmidt.github.io/)

## Technologies Used
- **Excel**: Importing the dataset.
- **Power BI**: Power Query cleaning, modeling and report creation.

## Process
**Import**
- Imported tables from excel

**Power Query**
- Converted data types of columns 
- Substituted N/A and null values 
- Trimmed text columns
- Standardized terms
- Used first row as header 
- Rounded values

**Modeling**
- Created many to one relationships between fact table and dimensional tables
- Hid all ID columns from the report view
- Set date table as universal date table
- Created DAX measures of sales data
<img src="images/total_revenue.jpg" alt="Calculating total revenue" width="300">
<img src="images/total_quantity.jpg" alt="Calculating total quantity" width="300">
<img src="images/revenue_ytd.jpg" alt="Calculating revenue YTD" width="500">
<img src="images/revenue_total.jpg" alt="Calculating revenue % of total" width="650">
<img src="images/high_revenue.jpg" alt="Calculating count of high revenue customers" width="800">
<img src="images/average_discount.jpg" alt="Calculating average sales discount" width="350">

- Create a calculated order size column based on quantity purchased by the customer
<img src="images/order_size.jpg" alt="Calculating order size column" width="300">

**Reporting**
- Made an overview page with cards of metrics, a line chart of revenue generated each month and a treemap of revenue generated for each category with drilldown functionality.
- Made a products page with bar charts of revenue by product and quantity by product and a matrix showing metrics by category with drilldown functionality.
- Made a customers page with a column chart showing quantity order sizes, circle chart for revenue by region and a donut chart for the average discount of purchase by gender.
- Made slicers to filter by month, age and subcategory.
- Added tooltips to visuals to extend the information shown on hover. 
- Styled and orchestrated visuals for accessibility. 

## Final Report
**Overview of Central Metrics**
<img src="images/Overview.jpg" alt="Overview of central metrics" width="1000">

**Product Metrics**
<img src="images/Products.jpg" alt="Product metrics" width="1000">

**Customer Metrics**
<img src="images/Customers.jpg" alt="Customer metrics" width="1000">
