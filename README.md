# yoga-app-serverless

A serverless Yoga Learning App built on AWS.  
Users can browse yoga poses, learn their benefits, and take quizzes.  
The application uses a fully serverless backend and a static frontend hosted on S3 + CloudFront.

---

## Features
- Browse yoga poses with images and descriptions
- Learn pose benefits and difficulty levels
- Take randomized yoga quizzes
- Track learning progress
- Secure login with Amazon Cognito
- Fully serverless backend (API Gateway + Lambda + DynamoDB)
- Infrastructure managed with AWS CDK (TypeScript)

---

## Architecture Overview
- **Frontend**: React + TypeScript (S3 + CloudFront)
- **Backend**: API Gateway + Lambda (Python/FastAPI)
- **Database**: DynamoDB (YogaPoses, UserProgress)
- **Authentication**: Amazon Cognito
- **Storage**: S3 (pose images)
- **IaC**: AWS CDK (TypeScript)
- **CI/CD**: GitHub Actions

---

## Directory Structure (planned)
yoga-app-serverless/

├── frontend/        # React + TypeScript

├── backend/         # FastAPI Lambda code

├── infra/           # AWS CDK (TypeScript)

├── assets/          # Yoga pose images

└── README.md

---

## Deployment (CDK)
cd infra
npm install
cdk bootstrap
cdk deploy

---

## Status
This project is under active development.  
Infrastructure (CDK) → Backend (Lambda/FastAPI) → Frontend (React) will be built step-by-step.
