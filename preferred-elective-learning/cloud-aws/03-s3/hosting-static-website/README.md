# Hosting a Static Website on Amazon S3

## Introduction

Amazon Simple Storage Service (Amazon S3) is a highly scalable, durable, and secure object storage service provided by AWS. While S3 is primarily used to store files such as images, videos, documents, and backups, it also provides a feature called **Static Website Hosting**, which allows users to host static websites directly from an S3 bucket.

A static website consists of files that are delivered to users exactly as stored. These files typically include:

* HTML files
* CSS files
* JavaScript files
* Images
* Videos
* Fonts
* Documents

Examples of static websites:

* Personal portfolios
* Resume websites
* Company landing pages
* Documentation sites
* Product showcase websites

Since static websites do not require server-side processing, Amazon S3 is a cost-effective and easy-to-manage hosting solution.

---

# Learning Objectives

After completing this project, you will be able to:

* Understand Amazon S3 Static Website Hosting.
* Create and configure an S3 bucket.
* Upload website files to S3.
* Enable Static Website Hosting.
* Configure bucket permissions.
* Make website files publicly accessible.
* Access a website through an S3 endpoint URL.
* Troubleshoot common hosting errors.

---

# What is Amazon S3?

Amazon S3 (Simple Storage Service) is an object storage service that allows users to store and retrieve any amount of data from anywhere on the internet.

### Key Features

* High durability (99.999999999% durability)
* High availability
* Scalability
* Security
* Low cost
* Global accessibility

### Common Uses

* Backup and recovery
* Data archiving
* Application hosting
* Static website hosting
* Media storage
* Data lakes

---

# What is Static Website Hosting?

Static Website Hosting is an Amazon S3 feature that allows a bucket to behave like a web server and serve website content directly to users.

Normally, S3 stores files only.

When Static Website Hosting is enabled:

* S3 serves HTML pages.
* S3 serves images and videos.
* S3 automatically loads the default page.
* Users can access the website through a public URL.

---

# Project Structure

Example website files:

```text
website/
│
├── index.html
├── about.html
├── contact.html
├── css/
│   └── style.css
├── images/
│   └── logo.png
└── js/
    └── script.js
```

### Purpose of Each File

| File         | Purpose               |
| ------------ | --------------------- |
| index.html   | Main page             |
| about.html   | About page            |
| contact.html | Contact page          |
| style.css    | Website styling       |
| logo.png     | Website image         |
| script.js    | Website functionality |

---

# Architecture Diagram

```text
                 User Browser
                       │
                       ▼
              Website Endpoint URL
                       │
                       ▼
             Amazon S3 Static Hosting
                       │
                       ▼
                 S3 Bucket
                       │
      ┌─────────────────────────┐
      │ index.html              │
      │ images/logo.png         │
      │ css/style.css           │
      │ js/script.js            │
      └─────────────────────────┘
```

---

# Step 1: Login to AWS Management Console

### What is AWS Management Console?

The AWS Management Console is a web-based interface used to manage AWS services.

### Procedure

1. Open AWS Console.
2. Enter username/email.
3. Enter password.
4. Sign in.
5. Search for S3 in the search bar.
6. Open Amazon S3.

### Result

You will be redirected to the Amazon S3 Dashboard.

---

# Step 2: Create an S3 Bucket

### What is a Bucket?

A bucket is a container used to store objects (files) in Amazon S3.

### Procedure

1. Click **Create Bucket**.
2. Enter a unique bucket name.

Example:

```text
aws-made-easy-website
```

3. Select Region.

Example:

```text
Asia Pacific (Mumbai) ap-south-1
```

4. Leave other settings as default.
5. Click Create Bucket.

### Result

Bucket created successfully.

---

# Step 3: Upload Website Files

### Procedure

1. Open the bucket.
2. Click Upload.
3. Select files.

Example:

```text
index.html
logo.png
style.css
```

4. Click Upload.

### Result

Files are stored in the bucket.

---

# Step 4: Test the Bucket

At this stage:

* Files exist in S3.
* Website hosting is not enabled.

If you try to access files publicly, you may see:

```text
Access Denied
```

This happens because S3 blocks public access by default.

---

# Step 5: Enable Static Website Hosting

### Why is this Required?

Without enabling this feature, S3 behaves only as a storage service.

Enabling Static Website Hosting turns S3 into a simple web server.

### Procedure

1. Open Bucket.
2. Click Properties.
3. Scroll to Static Website Hosting.
4. Click Edit.
5. Select Enable.

Specify:

```text
Index document:
index.html
```

Optional:

```text
Error document:
error.html
```

6. Save changes.

### Result

AWS generates a Website Endpoint URL.

Example:

```text
http://aws-made-easy-website.s3-website-ap-south-1.amazonaws.com
```

---

# Step 6: Understanding the Index Document

The index document is the first page displayed when a user visits the website.

Example:

```text
index.html
```

Browser Request:

```text
http://website-url
```

AWS Automatically Loads:

```text
index.html
```

Without index.html:

```text
404 Error
```

may occur.

---

# Step 7: Configure Block Public Access

### What is Block Public Access?

AWS protects your data by preventing public access.

By default:

```text
Public Access = Blocked
```

### Procedure

1. Open Bucket.
2. Go to Permissions.
3. Find Block Public Access.
4. Click Edit.
5. Uncheck:

```text
Block all public access
```

6. Confirm warning.
7. Save.

### Result

Bucket can now accept public permissions.

---

# Step 8: Configure Object Ownership

### What is Object Ownership?

Object Ownership controls who owns files and whether ACLs can be used.

### ACL Meaning

ACL = Access Control List

ACLs allow file-level permissions.

### Procedure

1. Open Permissions.
2. Scroll to Object Ownership.
3. Click Edit.
4. Select:

```text
ACLs Enabled
```

5. Save.

### Result

Files can now be individually configured as public.

---

# Step 9: Make Objects Public

### Why?

Even after bucket permissions are changed, files remain private.

Each file needs public read permission.

### Procedure

1. Select all files.
2. Click Actions.
3. Choose Make Public.

Permission Applied:

```text
Public Read
```

### Result

Anyone on the internet can access the files.

---

# Step 10: Access the Website

Go to:

```text
Properties
→ Static Website Hosting
→ Website Endpoint
```

Example:

```text
http://aws-made-easy-website.s3-website-ap-south-1.amazonaws.com
```

Open the URL in a browser.

### Result

Website loads successfully.

---

# Common Errors and Solutions

## Error 1: Access Denied

### Cause

* Bucket not public
* Files not public
* ACLs disabled

### Solution

* Disable Block Public Access
* Enable ACLs
* Make objects public

---

## Error 2: 404 Not Found

### Cause

```text
index.html missing
```

### Solution

Upload index.html and configure it as the Index Document.

---

## Error 3: Website Not Loading

### Cause

Static Hosting disabled.

### Solution

Enable Static Website Hosting.

---

# Security Considerations

When hosting websites publicly:

* Only make website files public.
* Do not upload confidential files.
* Use least privilege access.
* Enable versioning.
* Monitor bucket activity.

---

# Advantages of Amazon S3 Static Website Hosting

1. Low Cost
2. Highly Available
3. Scalable
4. Easy to Configure
5. No Server Management
6. Global Access
7. Integration with CloudFront

---

# Limitations

| Supported  | Not Supported   |
| ---------- | --------------- |
| HTML       | PHP             |
| CSS        | Java            |
| JavaScript | Spring Boot     |
| Images     | Node.js Backend |
| Videos     | Databases       |

S3 can host only static content.

---

# Real-World Applications

* Portfolio Websites
* Resume Websites
* Company Landing Pages
* Product Pages
* Event Websites
* Documentation Sites
* Educational Websites

---

# Interview Questions

### What is Amazon S3?

Amazon S3 is an object storage service used to store and retrieve data from anywhere on the internet.

### What is Static Website Hosting?

A feature that allows an S3 bucket to serve website content as a web server.

### Why do we disable Block Public Access?

To allow users on the internet to access website files.

### What is an Index Document?

The default webpage loaded when a user visits a website.

### What is ACL?

Access Control List, used to define permissions for S3 objects.

### Can S3 host dynamic websites?

No. S3 supports only static websites.

### What is the Website Endpoint?

A URL generated by AWS that allows users to access the hosted website.

---

# Conclusion

Amazon S3 Static Website Hosting is one of the simplest ways to deploy a website on AWS. By creating an S3 bucket, uploading website files, enabling static website hosting, configuring public access permissions, and making objects publicly readable, a fully functional static website can be hosted without managing any servers.

This project helps beginners understand core AWS concepts such as S3 buckets, object storage, permissions, ACLs, public access settings, and website deployment, making it an excellent starting point for AWS Cloud Practitioner and AWS Solutions Architect learning paths.
