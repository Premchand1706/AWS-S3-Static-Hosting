from pathlib import Path

content = """# AWS S3 Static Website Hosting

A simple cloud deployment project demonstrating how to host a static website using **Amazon Simple Storage Service (Amazon S3)**. The website is uploaded as an HTML file and served through the S3 static website endpoint.

## Project Overview

This project demonstrates the basic process of publishing a static webpage on AWS without configuring or maintaining a traditional web server.

### Objectives

- Create and configure an Amazon S3 bucket.
- Upload the website's `index.html` file.
- Configure bucket permissions for website access.
- Enable static website hosting.
- Access and verify the published webpage using the S3 website endpoint.

## Technologies Used

- **Amazon S3** — stores the website files and serves the static content.
- **AWS Management Console** — used to configure the bucket and hosting settings.
- **HTML** — provides the webpage content.

## Implementation Steps

1. **Open Amazon S3**  
   Sign in to the AWS Management Console and open the Amazon S3 service.

2. **Create an S3 bucket**  
   Create a bucket to store the website files. In this implementation, the bucket name shown in the screenshots is `static-website-29-10`.

3. **Upload the website file**  
   Open the bucket's **Objects** section and upload the `index.html` file.

4. **Configure the bucket policy**  
   Configure the bucket policy to allow the `s3:GetObject` action for the website object. This allows visitors to read the webpage when public access is intentionally enabled.

5. **Enable static website hosting**  
   Open the bucket's **Properties** section, find **Static website hosting**, enable it, and save the configuration.

6. **Open the website endpoint**  
   Copy the website endpoint displayed in the static website hosting settings and open it in a browser.

7. **Verify the deployment**  
   Confirm that the webpage loads and displays the message **“Welcome to My Website!”**.

## Expected Result

The `index.html` file is stored in Amazon S3 and served through the S3 static website endpoint. The implementation screenshots show a successful file upload, enabled static website hosting, and the webpage opening in a browser.

## Repository Structure

```text
AWS-S3-Static-Hosting/
└── index.html
```

*The structure above shows the main website file used in this project. Add or update the tree if your repository contains additional files.*

## Security Considerations

- Public read access should be enabled only when the website content is intended to be public.
- Do not store credentials, passwords, private documents, or sensitive information in a publicly accessible bucket.
- For production deployments, consider using Amazon CloudFront with HTTPS and a private S3 bucket.
- Review AWS permissions carefully to avoid granting unnecessary access.

## Learning Outcomes

Through this project, I gained practical experience with:

- Creating and managing an S3 bucket.
- Uploading website files to AWS.
- Configuring bucket policies and object read permissions.
- Enabling static website hosting.
- Testing a deployed webpage through its website endpoint.

## Project Repository

[View the source code on GitHub](https://github.com/Premchand1706/AWS-S3-Static-Hosting)

---

**Note:** The bucket name above is the one visible in the provided screenshots. S3 bucket names are globally unique, so another user may need to choose a different name when reproducing this project.
"""
path = Path("/mnt/data/README.md")
path.write_text(content, encoding="utf-8")
print(f"Professional README created at: {path}")
