# AWS S3 Static Website Hosting

This project demonstrates how to configure a static website using AWS S3 bucket.

## Project Structure
├── README.md
├── bucket-policy.json
└── index.html

## Configuration Steps

1. **Create S3 Bucket**
   - Log in to AWS Console
   - Navigate to S3 service
   - Create a new bucket with "my-static-website-bucket-zhengzheng"

2. **Upload Website Files**
   - Upload `index.html` to my bucket

3. **Enable Static Website Hosting**
   - Go to bucket Properties
   - Select "Static website hosting"
   - Choose "Enable"
   - Specify `index.html` as the Index document

4. **Set Bucket Permissions**
   - Apply the bucket policy from `bucket-policy.json`

## Accessing My Website
`http://my-static-website-bucket-zhengzheng.s3-website.ca-central-1.amazonaws.com`

