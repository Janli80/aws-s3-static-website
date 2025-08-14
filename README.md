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
   - Create a new bucket with appropriate name

2. **Upload Website Files**
   - Upload `index.html` and any other assets to your bucket

3. **Enable Static Website Hosting**
   - Go to bucket Properties
   - Select "Static website hosting"
   - Choose "Enable"
   - Specify `index.html` as the Index document

4. **Set Bucket Permissions**
   - Apply the bucket policy from `bucket-policy.json`
   - Replace `my-static-website-bucket` with your actual bucket name

## Accessing Your Website

After configuration, your website will be available at the S3 website endpoint:

`http://<your-bucket-name>.s3-website-<aws-region>.amazonaws.com`

You can find the exact URL in AWS Console:
1. Go to your S3 bucket
2. Navigate to "Properties" tab
3. Look under "Static website hosting" section
4. Copy the "Endpoint" URL

Example (replace with your actual info):
`http://example-bucket.s3-website-us-east-1.amazonaws.com`

## Important Notes

- Make sure your bucket name is unique globally
- This configuration makes your bucket contents publicly readable
- For production use, consider adding CloudFront and Route53 for custom domain and HTTPS
