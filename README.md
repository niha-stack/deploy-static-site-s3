# deploy-static-site-s3
Explored AWS S3 static website hosting by publicly deploying a static asset (image) with proper bucket policy and access control.



# Objective
This project demonstrates how to use Amazon S3 (Simple Storage Service) to publicly host a static image using S3's static website hosting feature. The goal was to gain hands-on experience with basic AWS services, understand bucket configuration, and learn how static content is served over the internet through cloud infrastructure.



# Tools & Technologies
Amazon S3: Used to store the image and enable static website hosting.

AWS Console: For bucket creation, configuration, and policy management.

Bucket Policy: Written in JSON to allow public read access to the object.



# What i did

## Creating a bucket

### 1.Give it a unique name.

### 2.Choose a region (e.g., us-east-1).

![Fig 1](https://github.com/user-attachments/assets/0f7d2412-b521-45a8-bbeb-23a4039fa308)

### 3.Disabled “Block all public access”.

![Fig 2](https://github.com/user-attachments/assets/ec76234b-e77d-483f-9405-8627aa19df8e)

### 4.Bucket is created

![Fig 3](https://github.com/user-attachments/assets/47ab82a7-cf03-413e-bc20-f719f92b72d1)



## Upload Content 

### 1.Added a .png image to the bucket.

![Fig 4](https://github.com/user-attachments/assets/97f08b30-28ff-4830-aa2d-a6500ebf1bfa)



## Set Public Permissions

### 1.Go to bucket policy and click on edit


### 2.click on policy generator - it will navigate to other page

![Fig 5](https://github.com/user-attachments/assets/41ea62f0-4ccb-4512-a54e-fa00dd7d2a37)

### 3.Added a bucket policy to allow public GetObject access for all files in the bucket.

### 4.Copy the json code and paste it and save 
![Fig 6](https://github.com/user-attachments/assets/209effc9-7994-4835-b7f5-d7e99469901a)

![Fig 7](https://github.com/user-attachments/assets/72d3a8da-079a-49df-a86c-2c703b4e8a6b)



## Enable Static Website Host

### 1.Go to bucket properties and enable static website host , Mention the content name and save 
![Fig 8](https://github.com/user-attachments/assets/16e61449-2205-4461-8550-7a3f4bf723e5)



## Copy the url

![Fig 9](https://github.com/user-attachments/assets/0c0449a9-1512-4f46-9ec4-1cff28c2f6a6)

## Output

### 1.Accessed the Image via Public URL
![p10](https://github.com/user-attachments/assets/dc69b4f5-1387-4602-974b-dbeba2e71205)



# What i learned

### 1.How static website hosting works in S3.

### 2.How to configure public access safely using bucket policies.

### 3.The basics of object URLs and how AWS handles static content delivery.

### 4.Real-world example of serving content without needing a server or backend.





