# sql-time-Series-Analysis
sql
SELECT 
    date, 
    sales, 
    SUM(sales) OVER (ORDER BY date) AS running_total 
FROM time_series_data;
