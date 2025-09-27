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
 Month Name – The month name (January, February, …) has been extracted from the order date. This makes it easier to analyze month-wise sales trends and seasonal performance.

Week Day Name – The weekday (Monday–Sunday) has been derived from the order date. This helps compare sales from weekdays versus weekends and is useful in identifying peak business days.
