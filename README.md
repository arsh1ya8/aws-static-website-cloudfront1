
# Personal CV Website – AWS S3 & CloudFront

A personal CV website hosted on Amazon S3 and delivered globally through Amazon CloudFront.

## Live Website

https://d16h1um7joi577.cloudfront.net

## Architecture

The website uses the following AWS services:

- **Amazon S3:** Stores the static website files (HTML, CSS, and image).
- **Amazon CloudFront:** Distributes website content through a global content delivery network.
- **Origin Access Control (OAC):** Allows CloudFront to access the private S3 bucket securely.
- **Amazon CloudWatch:** Used to explore available storage and distribution metrics.

## Technologies Used

- HTML
- CSS
- Amazon S3
- Amazon CloudFront
- Amazon CloudWatch

## Deployment Steps

1. Created an S3 bucket to store the website files.
2. Uploaded `index.html`, `index.css`, and `avatar.png`.
3. Kept public access blocked on the S3 bucket.
4. Created a CloudFront distribution using the S3 bucket as its origin.
5. Configured Origin Access Control (OAC).
6. Granted CloudFront access to the S3 bucket.
7. Configured `index.html` as the default root object.
8. Accessed the deployed website using the CloudFront distribution domain.

## Project Structure

```text
├── index.html
├── index.css
└── avatar.png
```

## Key Learnings

- Hosting static websites using Amazon S3.
- Configuring CloudFront distributions.
- Securing S3 origins using Origin Access Control.
- Understanding content delivery and caching.
- Exploring AWS CloudWatch metrics.

## Author

Syeda Arshiya

[GitHub](https://github.com/arsh1ya8)

## Deployment Screenshots

### Live Website
![Live Website](screenshots/website-live.png)

### Amazon S3 Bucket
![S3 Bucket](screenshots/s3-bucket.png)

### CloudFront Distribution
![CloudFront](screenshots/cloudfront-distribution.png)
