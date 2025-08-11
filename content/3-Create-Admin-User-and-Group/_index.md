---
title : "Setup Frontend on AWS"
date : "2024-01-01"
weight : 3 
chapter : false
pre : " <b> 3. </b> "
---
#### Access to S3
- Create S3 Bucket for frontend
![14](/images/aws/1.14.png?featherlight=false&width=90pc)
- Fill your name bucket
- Choose general type s3 
![15](/images/aws/1.15.png?featherlight=false&width=90pc)
- Unchoose Block all access
- Disable version
![16](/images/aws/1.16.png?featherlight=false&width=90pc)
- Choose first encryption type
- Enable bucket key
![17](/images/aws/1.17.png?featherlight=false&width=90pc)
- After finishing those steps you just click into s3 and upload your files
- Choose the file correctly then follow the steps below 
- When you finish click the link on s3 to make sure it works 
![18](/images/aws/1.18.png?featherlight=false&width=90pc)
- Access your File to upload all the file you need
![19](/images/aws/1.19.png?featherlight=false&width=90pc)
![20](/images/aws/1.20.png?featherlight=false&width=90pc)
- After created your S3 bucket click into it
- Find permission tag and scroll down
- Click edit 
![21](/images/aws/1.21.png?featherlight=false&width=90pc)
-Paste this code into S3 edit permission:
 {{% notice info %}}
     {
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::baker-frontend-2024/*"
        },
        {
            "Sid": "AllowCloudFrontServicePrincipal",
            "Effect": "Allow",
            "Principal": {
                "Service": "cloudfront.amazonaws.com"
            },
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::baker-frontend-2024/*",
            "Condition": {
                "ArnLike": {
                    "AWS:SourceArn": "arn:aws:cloudfront::235007105677:distribution/EXB54XU4GB8MK"
                }
            }
        }
    ]
    }
{{% /notice %}}
- Scroll down until you find a link on S3 bucket
![22](/workshop/images/aws/1.22.png)
![23](/workshop/images/aws/1.23.png)
![24](/workshop/images/aws/1.24.png)
![25](/workshop/images/aws/1.25.png)
- Next step going to CloudFront 
![26](/workshop/images/aws/1.26.png?featherlight=false&width=90pc)
![27](/workshop/images/aws/1.27.png?featherlight=false&width=90pc)
![28](/images/aws/1.28.png?featherlight=false&width=90pc)
- After finishing that click on the newest CloudFront you created
- Do
![29](/images/aws/1.29.png?featherlight=false&width=90pc)
![30](/images/aws/1.30.png?featherlight=false&width=90pc)

