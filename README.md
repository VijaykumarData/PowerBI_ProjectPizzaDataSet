# PowerBI_ProjectPizzaDataSet
Key Measures Implemented in the Pizza Sales Project

In this project, several DAX measures were created to derive meaningful business insights from the raw sales dataset. These measures help in analyzing sales performance, customer behavior, and overall business efficiency.

Measure Name	Formula (DAX)	Business Meaning
**Total Order Placed**	COUNTROWS(DISTINCT('pizzasproject pizza_sales'[order_id]))	Calculates the total number of unique orders placed by customers.

**Total Pizza Sold**	SUM('pizzasproject pizza_sales'[quantity])	Shows the total number of pizzas sold across all orders.

**Total Revenue**	SUM('pizzasproject pizza_sales'[total_price])	Represents the overall revenue generated from all pizza sales.

**Number of Orders Distinct**	DISTINCTCOUNT('pizzasproject pizza_sales'[order_id])	Counts distinct orders placed in the dataset (used in other KPIs).

**Average Order Value (AOV)**	[Total Revenue] / [number of orders distinct]	Gives the average revenue earned per order (indicates customer spending behavior).

**Average Pizza per Order**	[total Pizza sold] / [total order placed]	Calculates the average number of pizzas purchased per order (shows order size trend).

**Time Intelligence Columns Created**

**Month Name** – Order date se month ka naam (January, February, …) extract kiya gaya hai. Isse month-wise sales trends aur seasonal performance analyze karna easy ho jata hai.

**Week Day Name** – Order date se week day (Monday–Sunday) fetch kiya gaya hai. Ye column sales ko weekday vs weekend ke perspective se compare karne me madad karta hai aur peak business days identify karne me use hota hai.
