# TFS_Forecast
Auto ARIMA modeling of transaction services product group. The code consists of two part the first part looks at the predictability of a product group by assesing if they have reocurring business and the second part of the code looks at forecasting.


## Predictability of products
Sales are dived into monthly buckets and a three year period is defined as assesment period. If these months are seen as elements in and array we look at the product of the monthly sales for year-2, year-1 and year-now. We do this for all months from 1 till 12 and take the sum of all these products. Full score would be 10^3 times 12 so 12000.

## Auto arima modeling
For the very predictable products we see if we can make assumptions about expected purchases by running a auto arima model that determines the best arima parameters automatically.
