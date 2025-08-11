---
title : "Connect to MongoDB Atlas"
date : "2024-01-01"
weight : 3 
chapter : false
pre : " <b> 1.3 </b> "
---

#### Connect to mongoDB Atlas

**Go to MongoDB Atlas**
- 1.Configuration
    - Create MongoDB Account
    - Select build **Cluster**
    - Then **Create**
![5](/workshop/images/aws/1.5.png)

- 2.Setup your cluster
    - Name your **Cluster**
    - Choose **AWS Provider**
    - Region(Should choose along with your EC2 Region to avoid errors)
    - Then **Create**
![6](/workshop/images/aws/1.6.png)

- 3.Cluster connection
    - Install mongoDB in your Command prompt
    - Copy the link to the Cluster, **<db_username>:<db_password>@cluster0…** replace **<db_username>** and **<db_password>** with username and password on the Set up connection page above. Make sure this link to connect to the database and EC2.
![7](/workshop/images/aws/1.7.png)


