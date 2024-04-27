---
title : "RDS Connector"
date :  "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 2.2 </b> "
---

## RDS Connector
With Athena Jdbc Connector, the following databases are supported:

* MySQL
* PostgreSQL
* Redshift

For detailed information about Amazon Athena Jdbc Connector, refer [here](https://docs.aws.amazon.com/athena/latest/ug/connectors-postgresql.html) .

Athena PostgreSQL Connector can be installed as outlined below.

1. Create data source:
   - Access the [Athena Data sources](https://us-east-1.console.aws.amazon.com/athena/home?region=us-east-1#/data-sources).
   - Choose **Create data source**
   - If you need create Lambda look at 2.
   
   ![Image](/repo_pmt_ws-002/images/4/402.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-002/images/4/404.png?featherlight=false&width=90pc)
   
2. Create Lambda function:
   
   ![Image](/repo_pmt_ws-002/images/4/405.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-002/images/4/406.png?featherlight=false&width=90pc)

   - Update permission of IAM role for Lambda
   
   ![Image](/repo_pmt_ws-002/images/4/407.png?featherlight=false&width=90pc)

   - Update connection string
   
   ![Image](/repo_pmt_ws-002/images/4/408.png?featherlight=false&width=90pc)

   -  Create VPC endpoint( 1 gateway endpoint for S3, 1 interface endpoint for Secret Manager)

   ![Image](/repo_pmt_ws-002/images/4/502.png?featherlight=false&width=90pc)
   
3. Query
   - Check connection of data source

   ![Image](/repo_pmt_ws-002/images/4/409.png?featherlight=false&width=90pc)
   - Query RDS in Athena
   
   ![Image](/repo_pmt_ws-002/images/4/410.png?featherlight=false&width=90pc)

