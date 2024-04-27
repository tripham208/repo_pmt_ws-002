---
title : "Clean up resources"
date : "`r Sys.Date()`"
weight : 4
chapter : false
pre : " <b> 4. </b> "
---
## Cleanup

We will proceed to delete the resources in the following order:

When you have finished with this workshop, remember to clean up all those AWS resources that you created using AWS CloudFormation.

Follow the steps below for clean up:
### Athena Spark

- You would need to manually go and empty the S3Bucket athena-spark-workshop created by the CloudFormation as S3 bucket can only be deleted by CloudFormation once it's empty.

- Use the AWS CloudFormation console or AWS CLI to delete the stack named Athena-Spark-Workshop.

   ![Image](/repo_pmt_ws-002/images/5/501.png?featherlight=false&width=90pc)
### Athena Federation

1. [ ] Delete VPC endpoint

   ![Image](/repo_pmt_ws-002/images/5/503.png?featherlight=false&width=90pc)
2. [ ] Delete Database in RDS

   ![Image](/repo_pmt_ws-002/images/5/504.png?featherlight=false&width=90pc)
3. [ ] Delete Lambda function

   ![Image](/repo_pmt_ws-002/images/5/501.png?featherlight=false&width=90pc)
4. [ ] Delete IAM Role of Lambda
5. [ ] You would need to manually go and empty the S3Bucket created for Athena then delete it.
