# talend-warehousing
ETL using Talend Open Studio from OLTP to OLAP Warehouse

Project uses Northwind Operational Database in SQL Server and constructs ETL pipeline to OLAP with the following dimensions:
-> Customer
-> Employee
-> Time
-> Product

2 fact tables have been used. 
First one uses Orders table to calculate total price of orders with respect to above mentioned dimensions:
![image](https://github.com/danishminhas1/talend-warehousing/assets/53962550/2e2d9f27-fe72-48c5-af51-4b95d7c25db1)

Tables have been matched using "tmap" component as such:
![image](https://github.com/danishminhas1/talend-warehousing/assets/53962550/dfc1bbe3-6897-42b1-821e-24dceabf7b1f)


Second fact table calculates the total number of orders, including the delivered and undelivered orders:
![image](https://github.com/danishminhas1/talend-warehousing/assets/53962550/3fff1935-817f-4e0e-adb1-63751b469fbb)

Tables have been matched using "tmap" component as such:
![image](https://github.com/danishminhas1/talend-warehousing/assets/53962550/8301a59e-c8a4-4c81-a2fa-d12d0570175f)





