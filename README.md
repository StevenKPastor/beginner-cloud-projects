# beginner-cloud-projects

# 🚀 Project Title – Example: Text Narrator Using Amazon Polly

## 📌 Overview
Developing a text narrator using Amazon Polly which would be able to read a piece of text and will be uploaded in Amazon S3 bucket. This text will be converted into speech and I can adjust the voice, pitch, and speed parameters. 

## 🏗️ Architecture
![Architecture Diagram](./diagrams/architecture.png)

**Services Used**
-Amazon Polly - Converts text to speech 
-Amazon S3 - stores text files that will be converted into speech
-AWS IAM - Access Control
-AWS Management Console - Manages accounts and configured Amazon Polly

## ⚙️ Deployment
Steps to recreate:
1. Explored Amaazon Polly 
2. Created an IAM role and placed policies 
  a. AmazonPollyFullAccess
  b. AmazonS3FullAccess
  c. AWSLambdaBasicExecutionRole
4. Creating an S3 Bucket to store text files
5. Access via CloudFront URL

## 🔒 Security Considerations
- IAM least privilege for Lambda and CI/CD
- S3 bucket private with public access only via CloudFront
- Encryption at rest for DynamoDB and S3
- CloudWatch alarms for 5xx errors and throttling

## 📊 Results
- Fully serverless with automatic scaling
- Deployment completed in under N minutes via IaC
- Est. monthly cost: AWS Free Tier

## 🧪 Testing
- Postman collection for API endpoints in `/docs`
- Basic integration test script in `/scripts`

## 📚 Lessons Learned
- Key takeaways about service limits, IAM pitfalls, or IaC modules

## ▶️ Repo Map
