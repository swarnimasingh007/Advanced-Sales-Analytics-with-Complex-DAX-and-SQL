SELECT * FROM coffee_shop_sales

SELECT COUNT(transaction_id) AS Total_Sales
FROM coffee_shop_sales
WHERE
MONTH(transaction_date) = 5 -- March Month



SELECT
	MONTH(transaction_date) As month,
    ROUND(SUM(unit_price * transaction_qty)) As total_sales,
    (SUM(unit_price * transaction_qty) - LAG(SUM(unit_price * transaction_qty), 1)
    OVER (ORDER BY MONTH(transaction_date))) / LAG(SUM(unit_price * transaction_qty), 1)
	OVER (ORDER BY MONTH(transaction_date)) * 100 As mom_increase_percentage
FROM
	coffee_shop_sales
WHERE
	MONTH(transaction_date) IN (4, 5) -- for months of april and may
GROUP BY 
	MONTH(transaction_date)
    
    
    SELECT
	MONTH(transaction_date) As month,
    ROUND(COUNT(unit_price * transaction_id)) As total_sales,
    (COUNT(unit_price * transaction_id) - LAG(COUNT(unit_price * transaction_id), 1)
    OVER (ORDER BY MONTH(transaction_date))) / LAG(COUNT(unit_price * transaction_id), 1)
	OVER (ORDER BY MONTH(transaction_date)) * 100 As mom_increase_percentage
FROM
	coffee_shop_sales
WHERE
	MONTH(transaction_date) IN (4, 5) -- for months of april and may
GROUP BY 
	MONTH(transaction_date)
    

SELECT SUM(transaction_qty) AS Total_Quantity_Sold
FROM coffee_shop_sales
WHERE
MONTH(transaction_date) = 6 -- june Month

SELECT
    SUM(unit_price * transaction_qty) AS Total_sales,
    SUM(transaction_qty) AS Total_Qty_Sold,
    COUNT(transaction_id) AS Total_Orders
FROM coffee_shop_sales
WHERE 
    transaction_date = '2023-05-18'




    
