# 📌 Day 1 – Static Website Hosting on AWS  

## 🔥 Project Goal  
Host a static website on **Amazon S3**, configure a custom domain with **Route 53**, and use **CloudFront CDN** for faster, secure global delivery.  

---

## 🛠️ Services Used  
- **Amazon S3** – Store static website files (HTML, CSS, JS).  
- **Amazon Route 53** – Manage custom domain (DNS mapping).  
- **Amazon CloudFront** – Content Delivery Network (CDN) for caching, HTTPS, and performance.  
- **IAM** – Manage permissions for S3 access.  

---

## 📂 Steps to Implement  

### 1️⃣ Create and Configure S3 Bucket
- Go to **S3 Console** → Create bucket (name it like `aws-webhosting-day1`).  
- Uncheck **Block all public access**.  
- Enable **Static Website Hosting**.  
- Upload your website files (`index.html`, `style.css`, etc.).  

### 2️⃣ Set Permissions  
- Add a **Bucket Policy** for public read:  

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::aws-webhosting-day1/*"
    }
  ]
}
