# Hosting a Static Website on Amazon S3

## Overview

Amazon S3 (Simple Storage Service) provides a simple and cost-effective way to host static websites. Static websites consist of HTML, CSS, JavaScript, images, videos, and other files that do not require server-side processing.

This project demonstrates how to host a static website using Amazon S3 by creating a bucket, uploading website files, configuring static website hosting, and setting the required permissions.

---

# Prerequisites

Before starting, ensure you have:

* An AWS Account
* Access to the AWS Management Console
* Basic knowledge of HTML
* Website files ready for deployment

Example website files:

```
website/
│
├── index.html
├── logo.png
└── styles.css
```

---

# Architecture

```
User Browser
      │
      ▼
Amazon S3 Bucket
      │
      ▼
Static Website Hosting
      │
      ▼
Website Content Displayed
```

---

# Step 1: Sign in to AWS Management Console

1. Open the AWS Management Console.
2. Log in using your AWS credentials.
3. Search for **S3** in the services search bar.
4. Open the Amazon S3 dashboard.

---

# Step 2: Create an S3 Bucket

1. Click **Create bucket**.
2. Enter a unique bucket name.

Example:

```
aws-made-easy-website
```

3. Select the desired AWS Region.
4. Leave the remaining settings as default.
5. Click **Create bucket**.

Result:

```
Bucket created successfully.
```

---

# Step 3: Upload Website Files

1. Open the newly created bucket.
2. Click **Upload**.
3. Add your website files.

Example:

```
index.html
logo.png
styles.css
```

4. Click **Upload**.

Result:

```
Files stored inside the bucket.
```

---

# Step 4: Enable Static Website Hosting

1. Open the bucket.
2. Go to the **Properties** tab.
3. Scroll down to **Static Website Hosting**.
4. Click **Edit**.
5. Select:

```
Enable
```

6. Specify:

```
Index document: index.html
Error document: (optional)
```

7. Save changes.

Result:

```
Website endpoint URL generated.
```

Example:

```
http://aws-made-easy-website.s3-website-ap-south-1.amazonaws.com
```

---

# Step 5: Disable Block Public Access

By default, Amazon S3 blocks public access to improve security.

To make the website accessible:

1. Open the bucket.
2. Go to the **Permissions** tab.
3. Click **Edit** under **Block Public Access**.
4. Uncheck:

```
Block all public access
```

5. Confirm the warning.
6. Save changes.

Result:

```
Bucket can now accept public permissions.
```

---

# Step 6: Configure Object Ownership

AWS may disable ACLs by default.

To allow public file permissions:

1. Open **Permissions**.
2. Scroll to **Object Ownership**.
3. Click **Edit**.
4. Select:

```
ACLs Enabled
```

5. Save changes.

Result:

```
Object-level permissions can now be configured.
```

---

# Step 7: Make Website Files Public

1. Open the bucket.
2. Select all website files.
3. Click **Actions**.
4. Choose:

```
Make Public Using ACL
```

5. Confirm the action.

Result:

```
Files become publicly accessible.
```

---

# Step 8: Access the Website

1. Go to **Properties**.
2. Copy the generated website endpoint.

Example:

```
http://aws-made-easy-website.s3-website-ap-south-1.amazonaws.com
```

3. Open the URL in a browser.

Result:

```
Website loads successfully.
```

---

# Common Error: Access Denied

### Problem

```
Access Denied
```

### Possible Causes

* Static website hosting not enabled
* Block Public Access enabled
* Objects not public
* ACLs disabled
* Missing index.html file

### Solution

Verify:

✅ Static Website Hosting enabled

✅ index.html specified

✅ Public Access Block disabled

✅ ACLs enabled

✅ Files made public

---

# Key AWS Concepts

## Amazon S3 Bucket

A bucket is a container used to store files and objects in Amazon S3.

### Example

```
my-website-bucket
```

---

## Static Website Hosting

A feature that allows an S3 bucket to serve website content directly to users.

### Supported Content

* HTML
* CSS
* JavaScript
* Images
* Videos
* Documents

---

## Block Public Access

A security feature that prevents public access to S3 resources.

Purpose:

* Protect sensitive data
* Prevent accidental exposure

---

## Access Control List (ACL)

ACLs define permissions for individual objects.

Common Permission:

```
Public Read
```

Allows anyone on the internet to view the file.

---

## Index Document

The default page displayed when users access the website.

Example:

```
index.html
```

---

# Advantages of Hosting Static Websites on S3

* Low cost
* Highly scalable
* Easy deployment
* High availability
* No server management
* Global accessibility

---

# Limitations

* No server-side code execution
* No database support
* Cannot run PHP, Java Servlets, or Node.js applications
* Suitable only for static content

---

# Best Practices

* Use meaningful bucket names.
* Enable versioning for backup.
* Use CloudFront for faster delivery.
* Use HTTPS through CloudFront.
* Monitor usage with AWS CloudWatch.
* Follow least-privilege security practices.

---

# Real-World Use Cases

* Portfolio websites
* Resume websites
* Company landing pages
* Documentation websites
* Product showcase sites
* Educational websites

---

# Summary

Hosting a static website on Amazon S3 is one of the easiest ways to deploy web content on AWS. The process involves:

1. Creating an S3 bucket
2. Uploading website files
3. Enabling Static Website Hosting
4. Configuring public access
5. Making objects public
6. Accessing the website through the S3 endpoint

Amazon S3 provides a reliable, scalable, and cost-effective solution for hosting static websites without managing servers.
