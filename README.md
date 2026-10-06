# AWS Static Website with S3 & CloudFront

A static website hosted on **Amazon S3** and delivered worldwide through **Amazon CloudFront**. I built it to learn AWS basics: IAM, S3, CloudFront, HTTPS and caching.

## Live Demo

👉 https://d1qqy5foab4d46.cloudfront.net/

## How It Works

```text
User ──HTTPS──▶ CloudFront (CDN) ──OAC──▶ Private S3 bucket (index.html, style.css)
```

- **S3** stores the website files. The bucket is private, so nobody can reach it directly.
- **CloudFront** is the public entry point. It serves the site over HTTPS and caches it at edge locations, so pages load fast everywhere.
- **Origin Access Control (OAC)** lets only CloudFront read from the private bucket.

## Tech Used

- Amazon S3, Amazon CloudFront, AWS IAM
- HTML, CSS
- Git & GitHub


