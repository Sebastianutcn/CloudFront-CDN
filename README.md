# CloudFront-CDN
This repository contains Terraform code to provision a static website in an S3 bucket with CloudFront as a CDN for global content delivery.

**Files:**
1. [`s3.tf`](https://github.com/Sebastianutcn/host-static-website-s3/blob/main/main.tf) defines the infrastructure for hosting a static web app in an S3 bucket, including resources like the bucket, permissions, and static website hosting settings.
2. [`cloudfront.tf`](https://github.com/Sebastianutcn/host-static-website-s3/blob/main/main.tf) defines the CloudFront distribution.
3. [`provider.tf`](https://github.com/Sebastianutcn/host-static-website-s3/blob/main/main.tf) s used to configure the provider..
4. [`./src/index.html`](https://github.com/Sebastianutcn/host-static-website-s3/blob/main/src/index.html) is a simple HTML file.
5. [`./src/error.html`](https://github.com/Sebastianutcn/host-static-website-s3/blob/main/src/index.html) is a custom HTML page displayed when an error is encountered.

## Installation
- Terraform command to initialize the project
```
terraform init
```
* Terraform command to plan the changes and to check again the resources that were added, changed or deleted
```
terraform plan -out plan.out
```
- Terraform command to apply the changes
```
terraform apply plan.out --auto-approve
```

