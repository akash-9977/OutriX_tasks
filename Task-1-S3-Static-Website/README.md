# 🌐 Task 1: Static Website Deployment on AWS S3

## 📌 Project Overview

This project demonstrates how to deploy a static website using **Amazon S3**.  
I created a simple website using **HTML, CSS, and JavaScript**, uploaded the files to an **S3 bucket**, enabled **static website hosting**, configured **public access**, and tested the live website using the S3 website endpoint.

---

## 🎯 Task Objective

To host a static website using an **Amazon S3 bucket** with public access.

---

## 🛠️ Tools & Technologies Used

| Tool / Technology | Purpose |
|---|---|
| HTML | Website structure |
| CSS | Website styling |
| JavaScript | Basic interactivity |
| Amazon S3 | Static website hosting |
| AWS Console | Cloud configuration |
| GitHub | Project repository |

---

## ✨ Features

- Static website built with HTML, CSS, and JavaScript
- Hosted on Amazon S3
- Publicly accessible through an S3 website endpoint
- Custom `index.html` home page
- Custom `404.html` error page
- Basic JavaScript button interaction
- Clean and simple UI

---

## 📁 Project Structure

```text
Task-1-S3-Static-Website/
│
├── index.html
├── style.css
├── script.js
├── 404.html
└── README.md

🚀 Deployment Steps
1.Created a static website using HTML, CSS, and JavaScript.
2.Created an Amazon S3 bucket.
3.Uploaded website files to the S3 bucket.
4.Enabled Static Website Hosting in bucket properties.
5.Set index.html as the index document.
6.Set 404.html as the error document.
7.Disabled Block Public Access for the demo bucket.
8.Added a bucket policy to allow public read access.
9.Tested the website using the S3 website endpoint.

🔐 Bucket Policy Used
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::YOUR-BUCKET-NAME/*"
    }
  ]
}

🧪 Testing
The website was tested using the S3 static website endpoint.
Test cases performed:
Opened the website endpoint successfully
Verified that index.html loads properly
Checked CSS styling
Tested JavaScript button functionality
Tested custom 404.html error page

📚 Key Learnings
Through this task, I learned:
How Amazon S3 works as object storage
How to create and configure an S3 bucket
How to upload website files to S3
How to enable static website hosting
How to configure index and error documents
How bucket policies work
How public access is managed in AWS S3

🧠 Important Concepts
Concept	Explanation
Amazon S3	Object storage service used to store and retrieve files
Bucket	A container for storing objects/files
Object	A file stored inside an S3 bucket
Static Website	A website made with fixed files like HTML, CSS, and JavaScript
Bucket Policy	JSON-based permission rule used to control access
Index Document	Default page loaded when the website URL is opened
Error Document	Page shown when a requested file is not found

⚠️ Common Issues & Fixes
Issue	Possible Reason	Fix
403 Access Denied	Public access not configured	Disable Block Public Access and add bucket policy
404 Not Found	File missing or wrong file name	Check index.html and 404.html file names
CSS not loading	CSS file path issue	Ensure style.css is uploaded and linked correctly
Invalid bucket policy	Wrong bucket ARN	Use correct format: arn:aws:s3:::bucket-name/*

✅ Conclusion
This task helped me understand the basics of cloud storage, static website hosting, and public access configuration using AWS S3.
I successfully deployed and tested a static website using Amazon S3.
