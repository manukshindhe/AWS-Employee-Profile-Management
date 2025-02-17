📌 Project Overview

The AWS Employee Profile Management System is a cloud-based solution designed to manage employee profiles securely and efficiently. Employees can input their details, upload profile pictures, and retrieve their information. The project is hosted on AWS, ensuring high availability, security, and scalability.

🏗️ Features

Employee registration with Name, Location, Technology, Salary and image.
Secure profile photo uploads to AWS S3.
Automated email notifications upon successful uploads.
High availability with Elastic Load Balancing and Auto Scaling.
Secure data storage using RDS (MySQL) and DynamoDB.
Route 53 for custom domain mapping.
Automated event-driven workflows using AWS Lambda & SNS.

🛠️ AWS Services Used

VPC: Secure network architecture with public and private subnets.
EC2 & Auto Scaling: Application hosting and scaling.
Elastic Load Balancer (ELB): Distributes traffic efficiently.
RDS (MySQL): Stores employee details securely.
DynamoDB: Manages image metadata.
S3: Stores profile pictures and static web pages.
Route 53: Domain mapping and DNS management.
Lambda: Executes functions when a new file is uploaded to S3.
SNS (Simple Notification Service): Sends automated email notifications.

🚀 How to Deploy

1️⃣ Setup AWS Infrastructure

Create a VPC with public and private subnets.
Deploy EC2 instances for the application.
Setup an Auto Scaling Group for high availability.
Configure RDS (MySQL) for storing employee data.
Create an S3 Bucket for profile pictures and static content.
Setup Route 53 to map a custom domain to the Load Balancer.
Use IAM Roles to grant necessary permissions to EC2 instances.

2️⃣ Application Deployment

Upload the web application to EC2 instances.
Configure the database schema in RDS (MySQL).
Deploy Lambda functions to trigger SNS notifications on S3 uploads.
Set up security policies and IAM roles.

3️⃣ Testing & Monitoring

Upload a new employee profile and check S3 for images.
Ensure Route 53 directs traffic correctly.
Verify SNS notifications upon photo uploads.