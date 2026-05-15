# ☁️ AWS Serverless Inventory System

## 🏆 Pencapaian

Seleksi Internal LKS Cloud Computing SMK Negeri 4 Bandung 2026
Modul: Serverless Application

---

## 📋 Overview

Membangun sistem inventaris berbasis serverless di AWS.
Seluruh konfigurasi infrastruktur dilakukan secara mandiri
tanpa perlu mengelola server sama sekali.

Source code Lambda:
→ github.com/ZeitakuXIV/lksbdg-serverless

---

## 🏗️ Arsitektur

![Arsitektur](docs/architecture/arsitektur-aws-serverless-application.png)

---

## 📁 Struktur Repository

```
aws-serverless-inventory/
├── README.md
├── docs/
│   ├── api-reference.md
│   └── screenshots/
│       ├── architecture.png
│       ├── iam/
│       ├── dynamodb/
│       ├── s3/
│       ├── lambda/
│       ├── api-gateway/
│       └── testing/
└── policies/
    └── s3-bucket-policy.json
```

---

## ⚙️ Yang Dikonfigurasi

✅ IAM Role + Policy (AmazonDynamoDBFullAccess, AmazonS3FullAccess)
✅ DynamoDB Table (inventory, partition key: inventoryID)
✅ S3 Bucket + Public Bucket Policy
✅ Lambda Functions (5 functions: CRUD + List)
✅ Environment Variables di setiap Lambda
✅ API Gateway REST API + CORS
✅ Lambda Proxy Integration
✅ Deploy API ke stage "dev"
✅ Testing via Postman

---

## 🛠️ Tech Stack

![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-FF9900?style=flat&logo=awslambda&logoColor=white)
![DynamoDB](https://img.shields.io/badge/DynamoDB-4053D6?style=flat&logo=amazondynamodb&logoColor=white)
![API Gateway](https://img.shields.io/badge/API_Gateway-FF4F8B?style=flat&logo=amazonapigateway&logoColor=white)
![S3](https://img.shields.io/badge/Amazon_S3-569A31?style=flat&logo=amazons3&logoColor=white)
![IAM](https://img.shields.io/badge/AWS_IAM-DD344C?style=flat&logo=amazonaws&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

---

## 📸 Screenshots

### IAM Role - Permissions & Trust Policy

![IAM Role](docs/screenshots/iam/iam-role-policies.png)

### DynamoDB - Table Overview

![DynamoDB](docs/screenshots/dynamodb/dynamo-table.png)

### S3 Bucket - Bucket & Policy

![S3](docs/screenshots/s3/s3-bucket-config.png)

### Lambda Functions - All 5 Functions

![Lambda](docs/screenshots/lambda/lambda-func-list.png)

### API Gateway - Resources & Methods

![API Gateway](docs/screenshots/api-gateway/api-gateway-resource-tree.png)

### Testing via Postman

#### Postman Create Data

![Postman Create](docs/screenshots/testing/postman-create-success.png)

#### Postman List Data

![Postman List](docs/screenshots/testing/postman-list-data.png)

#### Postman Read Data

![Postman Read](docs/screenshots/testing/postman-get-data.png)

#### Postman Update Data

![Postman Update](docs/screenshots/testing/postman-update-success.png)

#### Postman Delete Data

![Postman Delete](docs/screenshots/testing/postman-delete-success.png)

---

<!-- ## 📝 Detail Konfigurasi

→ Lihat [docs/api-reference.md](docs/api-reference.md)

--- -->

## 📚 Referensi

→ [AWS Lambda](https://docs.aws.amazon.com/lambda/)  
→ [Amazon DynamoDB](https://docs.aws.amazon.com/dynamodb/)  
→ [Amazon API Gateway](https://docs.aws.amazon.com/apigateway/)  
→ [Amazon S3](https://docs.aws.amazon.com/s3/)  
→ [Source Code Lambda](https://github.com/ZeitakuXIV/lksbdg-serverless)
