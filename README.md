# s3-static-website-hosting

# 🚀 Static Website Hosting using Amazon S3

## 📌 Project Overview

This project demonstrates how to host a static website using Amazon S3 without using any servers.

The website is built using HTML and CSS and deployed on AWS S3 with public access enabled.

---

## 🎯 Objectives

* Create an S3 bucket
* Enable static website hosting
* Upload website files (HTML, CSS)
* Configure bucket policy for public access
* Access the website via S3 endpoint

---

## 🛠️ Technologies Used

* Amazon S3
* HTML
* CSS
* Git & GitHub

---

## 📂 Project Structure

```
s3-static-website/
│
├── index.html
├── style.css
├── images/
├── screenshots/
```

---

## ⚙️ Implementation Steps

### 1. Create S3 Bucket

* Created a bucket named `prashant-portfolio-site`
* Disabled Block Public Access

---

### 2. Enable Static Website Hosting

* Enabled static hosting from Properties tab
* Index document: `index.html`

---

### 3. Upload Website Files

* Uploaded HTML, CSS, and images to S3 bucket

---

### 4. Configure Bucket Policy

Applied the following policy to allow public access:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadAccess",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::prashant-portfolio-site/*"
    }
  ]
}
```

---

### 5. Access Website

The website is accessible using the S3 endpoint URL.

---

## 📸 Screenshots

### 🔹 S3 Bucket Created


### 🔹 Static Hosting Enabled


### 🔹 Bucket Policy


### 🔹 Website Output

---

## 🚀 Key Learnings

* Understanding of Amazon S3
* Static website hosting without servers
* Managing bucket policies and permissions
* Public access configuration

---

## ⚠️ Challenges Faced

* Bucket policy conflicts with Block Public Access
* Permission issues (IAM restrictions)

---

## 📌 Conclusion

This project demonstrates how to deploy a static website using AWS S3 efficiently without managing servers, making it cost-effective and scalable.

---

## 🔗 Future Improvements

* Add custom domain using Route 53
* Enable HTTPS using CloudFront
* Automate deployment using CI/CD

---

## 🙌 Author

**Prashant Giri**
