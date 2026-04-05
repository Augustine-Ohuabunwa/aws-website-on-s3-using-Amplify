📦 Static Website Deployment on AWS S3 with Amplify
Overview

This project demonstrates the deployment of a fully functional static website using Amazon S3 and AWS Amplify. It highlights practical expertise in cloud architecture, CI/CD pipelines, and AWS best practices for secure, scalable, and automated static website hosting.

Key Achievements:

Designed a production-ready static website hosting solution.
Automated deployment workflow using AWS Amplify.
Applied AWS security best practices: versioning, encryption, and controlled public access.
Delivered a live, accessible website with minimal manual intervention.
Technologies Used
AWS S3 – Static website hosting and object storage
AWS Amplify – CI/CD deployment automation
AWS Management Console – Infrastructure provisioning
HTML/CSS/JS – Static website content
Architecture Diagram

Below is a high-level view of the static website deployment architecture:


Diagram shows S3 bucket hosting, Amplify deployment, and optional CloudFront CDN for delivery.

Diagram Key Components:

Developer: Pushes code to Git repository
Amplify CI/CD: Detects changes, builds, and deploys artifacts
S3 Bucket: Stores static website files
CloudFront (optional): Distributes content globally with HTTPS
Users: Access website via Amplify-generated URL or custom domain
Deployment Steps
1. Create an S3 Bucket
Log in to AWS Management Console → S3 Dashboard → Create bucket.
Configure the bucket:
Type: General purpose
Name: Unique and compliant
ACL: Disabled
Block Public Access: Uncheck Block all public access
Versioning: Enabled
Encryption & Bucket Key: Enabled
Object Lock: Disabled
Click Create bucket.
2. Upload Website Files
Open the bucket → Upload → Add files.
Select index.html → Open → Upload → Close.
Verify the file appears in the bucket.

Screenshot Example:


3. Configure Amplify for CI/CD
In the bucket → Properties → Static website hosting → Create Amplify app.
Amplify creates an app and attaches a bucket policy.
Multiple apps can be managed under one Amplify environment.

Screenshot Example:


4. Deploy the Website
Select Amazon S3 as the deployment method.
Browse for your bucket/prefix if needed.
(Optional) Zip the content.
Click Save and deploy.
Copy the generated URL → verify website in a browser.

Screenshot Example:


Security & Best Practices
Versioning enabled for rollbacks and recovery.
Encryption enabled by default for data protection.
ACLs disabled, relying on IAM policies.
Public access controlled via Amplify policies; consider CloudFront OAC for production.
Professional Impact
Demonstrates ability to design scalable, production-ready cloud architecture.
Showcases practical CI/CD pipeline knowledge.
Highlights AWS service expertise and deployment automation skills.
Optional Enhancements
Add custom domain via Route 53.
Add CloudFront CDN for global performance.
Implement Git-based CI/CD for automated builds.
Enable logging, monitoring, and alerts for production readiness.

Outcome: Successfully deployed a secure, scalable static website with automated CI/CD on AWS, demonstrating proficiency in cloud architecture, DevOps, and AWS best practices.
