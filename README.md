# Stor-455-Methods-of-Data-Analysis
This is a collection of Assignments and Lecture Notes to show what I did in my Methods of Data Analysis class. The class focused on simple 
and multiple regression with quantitative and categorical variables, and how to use R to build Statistical regression models.
|API	|Public?	|Dependencies Touched	|Notes	|
|---	|---	|---	|---	|
|ExecuteSql	|Yes	|- Front-End Service
- DynamoDB: HttpEndpoint
- Aurora Serverless	|Implemented during Beta/Preview, will launch in GA as deprecated and eventually removed.	|
|ExecuteStatement
BeginTransaction
CommitTransaction
RollbackTransaction	|Yes	|- Front-End Service

Cold Start:
- DynamoDB: HttpEndpoint, AvailablePools, CustomerPools
- DAX: CustomerPools (write-through)
- Connection Pooling Fleet Instance (Pool process)

Hot Start:
- DAX: CustomerPools
- Connection Pooling Fleet Instance (Pool process)	|	|
|EnableHttpEndpoint
DescribeHttpEndpoint	|No	|- Control Plane Service
- DynamoDB: HttpEndpoint	|API is accessed via RDS SDK/CLI/Console and not directly	|
|DisableHttpEndpoint	|No	|- Control Plane Service
- DynamoDB: HttpEndpoint
- Connection Pooling Fleet (stop pools, if any)	|API is accessed via RDS SDK/CLI/Console and not directly	|
|	|	|	|	|
