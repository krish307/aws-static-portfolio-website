# AWS Static Portfolio Architecture

## Overview

This project hosts a static portfolio website using Amazon S3 and Amazon CloudFront.

## Architecture

```
User
   │
   ▼
CloudFront (HTTPS + CDN)
   │
   ▼
Amazon S3 Static Website Hosting
   │
   ▼
Portfolio Website
```

## Components

### Amazon S3
- Stores the website files.
- Hosts the static website.

### Amazon CloudFront
- Provides HTTPS.
- Delivers content globally.
- Improves loading speed through caching.

### GitHub
- Stores the project source code.
- Tracks version history.

### Browser
- Users access the website securely through CloudFront.

## Data Flow

1. User visits the CloudFront URL.
2. CloudFront checks its cache.
3. If needed, CloudFront fetches files from S3.
4. The website is delivered over HTTPS.