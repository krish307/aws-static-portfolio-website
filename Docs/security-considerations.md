# Security Considerations

## Overview

This project follows AWS security best practices appropriate for a static portfolio website.

---

## Security Measures

### Multi-Factor Authentication (MFA)

Enabled MFA for the AWS account to provide additional protection.

---

### IAM User

Created an IAM Administrator user for daily work instead of using the root account.

---

### Root Account

Used only for account setup and emergency access.

---

### CloudFront HTTPS

CloudFront provides HTTPS encryption between users and the website.

---

### Bucket Policy

Configured a bucket policy allowing public read access only because this is a public portfolio website.

---

### Public Access

Public access is intentionally enabled only for website content.

No sensitive data is stored inside the bucket.

---

### Future Improvements

- Origin Access Control (OAC)
- Private S3 Bucket
- AWS WAF
- Custom Domain
- ACM Certificate