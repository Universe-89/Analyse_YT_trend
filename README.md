
![image](https://github.com/tanmayks1999/Analyse_YT_trend/assets/37013559/97ecb68f-f61a-401f-9d81-27b6b5885787)
In this ETL pipeline we are going to source data from source system and show
analytics using AWS service . I have created a ETL pipeline which will take youtube
trending video data and then will create a report on it . Below are the reason I have
chosen these services .<br />
**Storage**<br />
For storage I have used S3 for storage because of its scalability and cost effectiveness .
Using S3 I have created a data lake which will have raw, cleaned and analytical data .
S3 also provides versioning which makes very convenient to roollback deleted data.<br />
**Data processing**<br />
Glue is already integrated with wide range of aws services . So we do need to manage
the underline infrastructure total cost of ownership is lower . Aws glue handles
configuration , provisioning and scaling of the resources required to run the ETL job .
So only have to pay for it while our job is running .<br />
**Data Catalogue**<br />
Glue Catalog and Crwaler helps in understanding how the data is presented . Crawler
will crwale through th data and will create metadata which is stored in table and
going to be used in authoring process of ETL job . Data Catlog contains data defination
, schemas etc and help mangae AWS Glue environment . It automatically computes
statistics and registers partition to make query run faster and cost effective .<br />
**Identity and Access Mangment**<br />
Different servies in AWS do not have access to interact with each other . AWS IAM
helps give only required permission and assign policy to a service so that it only
intercats with the services it should be . It can also create user and group and even
add multi factor authentication for added security .<br />
**Monitoring**<br />
Managing an ETL pipeline becomes difficulties and number of services grows . For
this we have AWS cloudwatch .We can monitor our entire application , network and
services . Can provide real time metrics and log and event data to take automated
actions .<br />
**Analysis**<br />
AWS Quicksight is already integrated with other AWS services . Using this quickly
data analysis dashboard can be created which we are grnerating using our ETL
pipeline . It has a in memory engine which can run query fast .<br />


Dashboard screenshorts

![image](https://github.com/tanmayks1999/Analyse_YT_trend/assets/37013559/fb8ab7e0-7789-49b7-8265-e1da5aaccc4c)

![image](https://github.com/tanmayks1999/Analyse_YT_trend/assets/37013559/516e1f2f-791c-49db-97a2-b712ffdf4942)
