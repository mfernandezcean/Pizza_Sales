## DAX:

Average:

```
Average Order per Day = 
DIVIDE( DISTINCTCOUNT('order_details'[order_id]), DISTINCTCOUNT(orders[date]))
```
Top 5 sales by Category: 
```
Top 5 Sales = 
VAR TopSalesTable = TOPN(5,
    SUMMARIZE('order_details', 'order_details'[pizza_id], "Total Sales", [Total Sales]),
    [Total Sales], DESC)
RETURN SUMX(TopSalesTable, [Total Sales])
```
Total Sales:
```
Total Sales = 
SUMX(
    'order_details',
     'order_details'[quantity] * RELATED('pizzas'[price]
     )
)
```
