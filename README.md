Total Payment = 
SUM('Baskin_Robins'[Payment Summary])

Payment YTD = 
TOTALYTD(
    [Total Payment],
    'Baskin_Robins'[shipping_date]
)

Avg Payment Per State =
AVERAGEX(
    VALUES('Stores'[State]),
    [Total Payment]
)


Dashboard Features

* KPI Cards for Total Revenue and YTD
* Sales by State (Bar Chart)
* Category-wise Sales (Column Chart)
* Payment Mode Distribution (Pie Chart)
* Quarterly Trend Analysis
* Interactive Filters (Slicers)
