# HR-Solution-Weather-Observation-Station-19
Solutions for MySQL and SQL Server

## PROBLEM
![image](https://github.com/user-attachments/assets/339872a0-4ab4-4315-8a99-29e8c31236aa)

[Euclidean Distance](https://en.wikipedia.org/wiki/Euclidean_distance)

## SQL SERVER:
SELECT CONVERT(DECIMAL(18, 4), (SQRT(POWER(MAX(LAT_N) - MIN(LAT_N), 2) + POWER(MAX(LONG_W) - MIN(LONG_W), 2))))
FROM STATION;

## MySQL:
SELECT ROUND(SQRT(POWER(MAX(LAT_N) - MIN(LAT_N), 2) + POWER(MAX(LONG_W) - MIN(LONG_W), 2)), 4)
FROM STATION;
