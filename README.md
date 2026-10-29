# AWS S3 Static Website Hosting

## Project Overview

This project demonstrates how I hosted a static website using Amazon Simple Storage Service (Amazon S3). I uploaded an HTML file to an S3 bucket, configured the required permissions, enabled static website hosting, and tested the website using the endpoint provided by AWS.

## Live Website

[Visit My Website](http://static-website-29-10.s3-website-us-east-1.amazonaws.com/)

## Technologies Used

- Amazon S3
- AWS Management Console
- HTML
- S3 Static Website Hosting

## Implementation Steps

### Step 1: Open Amazon S3

I logged in to the AWS Management Console and opened the Amazon S3 service.

### Step 2: Create an S3 Bucket

I created an S3 bucket named `static-website-29-10` to store my website files.

### Step 3: Open the Bucket

I opened the bucket and checked the Objects section. Initially, the bucket was empty.

### Step 4: Upload the Website File

I uploaded my `index.html` file to the bucket. After the upload was completed, I checked the status and confirmed that the file was uploaded successfully.

### Step 5: Configure the Bucket Policy

I opened the bucket permissions and edited the bucket policy to allow the `s3:GetObject` action. This allowed visitors to read the website file.

### Step 6: Enable Static Website Hosting

I opened the bucket's Properties section, selected Static website hosting, enabled the feature, and saved the settings.

### Step 7: Copy the Website Endpoint

After enabling static website hosting, I copied the website endpoint provided by AWS.

### Step 8: Test the Website

I opened the website endpoint in my browser. The webpage displayed the heading "Welcome to My Website!" and the message "This website is hosted on Amazon S3."

## Project Result

The website was successfully uploaded and hosted using Amazon S3. I configured the bucket policy, enabled static website hosting, and verified that the webpage was accessible through the S3 website endpoint.

## Skills Learned

- Creating and managing S3 buckets
- Uploading HTML files to AWS
- Configuring bucket policies and permissions
- Enabling static website hosting
- Testing a deployed website through its endpoint

## Security Note

The bucket policy allows public reading of the website file. Public access should only be enabled for content intended to be publicly available. Passwords, credentials, and private information should never be stored in a publicly accessible bucket.

