---
title : "RDS Connector"
date :  "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 2.2 </b> "
---

## RDS Connector
Với Athena Jdbc Connector, các cơ sở dữ liệu sau được hỗ trợ:

* MySQL
* PostgreSQL
* Redshift

Để biết thông tin chi tiết về Amazon Athena Jdbc Connector, hãy tham khảo [tại đây](https://docs.aws.amazon.com/athena/latest/ug/connectors-postgresql.html) .

Athena PostgreSQL Connector có thể được cài đặt như được nêu dưới đây.

1. Tạo nguồn dữ liệu:
   - Truy cập [Athena Data sources](https://us-east-1.console.aws.amazon.com/athena/home?region=us-east-1#/data-sources).
   - Chọn **Create data source**
   - Nếu bạn cần tạo Lambda, hãy xem 2.
   
   ![Image](/repo_pmt_ws-002/images/4/402.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-002/images/4/404.png?featherlight=false&width=90pc)
   
2. Tạo hàm Lambda:
   
   ![Image](/repo_pmt_ws-002/images/4/405.png?featherlight=false&width=90pc)

   ![Image](/repo_pmt_ws-002/images/4/406.png?featherlight=false&width=90pc)

   - Quyền cập nhật vai trò IAM cho Lambda
   
   ![Image](/repo_pmt_ws-002/images/4/407.png?featherlight=false&width=90pc)

   - Cập nhật connection string
   
   ![Image](/repo_pmt_ws-002/images/4/408.png?featherlight=false&width=90pc)

   -  Tạo VPC endpoint( 1 gateway endpoint cho S3, 1 interface endpoint cho Secret Manager)

   ![Image](/repo_pmt_ws-002/images/4/502.png?featherlight=false&width=90pc)
   
3. Truy vấn
   - Kiểm tra kết nối nguồn dữ liệu

   ![Image](/repo_pmt_ws-002/images/4/509.png?featherlight=false&width=90pc)
   - Truy vấn RDS trong Athena
   
   ![Image](/repo_pmt_ws-002/images/4/510.png?featherlight=false&width=90pc)

