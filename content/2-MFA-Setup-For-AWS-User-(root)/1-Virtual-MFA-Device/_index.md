---
title : "Setup EC2 environment for Backend"
date : "2024-01-01"
weight : 1 
chapter : false
pre : " <b> 2.1 </b> "
---
#### GET INTO EC2 CMD

1.**After you launch instance successfully, click on the newest one just created**
![8](/images/aws/1.8.png?featherlight=false&width=90pc)
   - Then click connect and you will get a EC2 Command Prompt on your new tab
![9](/images/aws/1.9.png?featherlight=false&width=90pc)
   - Then typing **sudo yum install -y nodejs** to download, it takes a while to download dont worry
   - After that type **sudo npm install -g pm2**
   - Type **sudo yum install -y git** and then wait for them downloading

![10](/images/aws/1.10.png?featherlight=false&width=90pc)
{{% notice info %}}
        **sudo yum install -y nodejs** 
        **sudo npm install -g pm2**
        **sudo yum install -y git**
    {{% /notice %}}
   - All commands are here!!!

2.**Configure MongoDB into EC2 instance**
   - Now link **Database from MongoDB** to EC2 command prompt and create an .env file
   - Type **echo "MONGO_URI=mongodb+srv://baker_user:<db_password>@<YOUR_CLUSTER>.tiggcso.mongodb.net/?retryWrites=true&w=majority&appName=<YOUR_CLUSTER> > .env**
   - Type **echo "JWT_SECRET=baker_jwt_secret_key_2024">> .env**
   - Type **echo "PORT=5001">> .env**
   - Type **echo "NODE_ENV=production">> .env**
   
![11](/images/aws/1.11.png?featherlight=false&width=90pc)
   -Check the version and then you ready to go
   {{% notice info %}}
      #Clone your backend repository 
      git clone [your-backend-repo-url] 
      cd [your-backend-directory] 
        **sudo yum install -y nodejs** 
        **sudo npm install -g pm2**
        **sudo yum install -y git**
    {{% /notice %}}
   - After cloning the project, continue running the following commands
   - Build application **npm run build**
   - Start with PM2:**pm2 start app.js --name "baker-backend"**
   - Save PM2 configuration: 
      - **pm2 save** 
      - **pm2 startups**
![12](/images/aws/1.12.png?featherlight=false&width=90pc)
- You can check by this commands:
- cd backend
- nano app.js
![13](/images/aws/1.13.png?featherlight=false&width=90pc)



