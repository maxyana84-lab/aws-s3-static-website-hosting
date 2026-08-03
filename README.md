# AWS S3 Static Website Hosting & Deployment

This project demonstrates the deployment and hosting of a lightweight static website using **Amazon S3 (Simple Storage Service)**, configuring public access policies, bucket hosting properties, and index/error document routing.

## 🎯 Objective
* Configure an **Amazon S3 Bucket** for static website hosting.
* Apply explicit **Bucket Policies** for controlled public read access (`s3:GetObject`).
* Configure **Index** and **Error** document routing.
* Test and verify web accessibility via the Amazon S3 Website Endpoint.

## 🏗 Architecture & Overview
1. **Storage Tier:** Amazon S3 Bucket hosting `index.html` and `error.html`.
2. **Access Control:** Adjusted "Block Public Access" settings with a custom JSON Bucket Policy for `s3:GetObject`.
3. **Endpoint Routing:** Amazon S3 handles HTTP routing for root domain and 404/Error fallbacks.

## 🛠 Implementation Steps
1. **Bucket Creation:** Created a globally unique S3 Bucket and adjusted public access settings.
2. **Static Hosting Activation:** Enabled Static Website Hosting in S3 Properties (`index.html` & `error.html`).
3. **Bucket Policy:** Applied JSON policy granting `s3:GetObject` permissions for public access:
