# S3 Static Website Project

A demonstration of hosting a static website using Amazon S3

## Overview

This project showcases how to deploy and host a static website using Amazon S3 bucket with public access configuration. 

## Architecture

- **Amazon S3**: Static file storage and web hosting

## Features

- Responsive design
- Fast loading times
- Cost-effective hosting solution
- Scalable architecture

## Prerequisites

- AWS Account
- Basic knowledge of HTML/CSS/JavaScript

## Setup Instructions

### 1. Create S3 Bucket

```bash
# Create bucket 

# Enable static website hosting
```

### 2. Configure Bucket Policy

Apply the following bucket policy to allow public read access:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::your-unique-bucket-name/*"
    }
  ]
}
```

### 3. Upload Website Files

```bash
# Upload all files to S3
```

### 4. Access Your Website

website will be available at:
```
http://vitsinpeace.s3-website-us-east-1.amazonaws.com/
```

## File Structure

```
├── index.html          # Main homepage
├── styles.css          # Stylesheet
├── script.js           # JavaScript functionality
├── images/             # Image assets
│   ├── logo.png
│   └── banner.jpg
└── README.md           # This file
```

## Cost Considerations

- S3 storage: ~$0.023 per GB/month
- S3 requests: ~$0.0004 per 1,000 requests
- Data transfer: First 1GB free per month

## Security Best Practices

- Use least privilege access
- Enable S3 bucket versioning
- Configure CloudTrail logging
- Implement proper CORS policies

## Monitoring

Monitor your website using:
- CloudWatch metrics
- S3 access logs

## Live Demo

🌐 [View Live Website](http://vitsinpeace.s3-website-us-east-1.amazonaws.com/)

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Amazon S3
