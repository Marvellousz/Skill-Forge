# Skill-Forge

A scalable, enterprise-grade Learning Management System (LMS) built with **Next.js**, **Node.js**, and **AWS**. This project demonstrates a modern full-stack architecture, robust authentication, seamless payment integration, and cloud deployment.

## Tech Stack

**Frontend**
- Next.js
- TypeScript
- Redux Toolkit
- Tailwind CSS
- Shadcn UI
- Framer Motion
- React Hook Form
- Zod
- Stripe

**Backend**
- Node.js
- Express.js
- Docker
- AWS Lambda
- AWS API Gateway
- DynamoDB
- AWS S3
- AWS CloudFront

**Authentication**
- Clerk

**Deployment**
- Vercel (Frontend)
- AWS (Backend)

---

## Features

- **Modern UI:** Responsive, accessible, and beautiful interface using Tailwind CSS and Shadcn UI.
- **Authentication:** Seamless user management with Clerk.
- **Course Management:** Create, edit, and view courses.
- **Billing & Payments:** Secure Stripe integration for payments and subscriptions.
- **Media Support:** Drag-and-drop uploads, video playback, and file management.
- **Serverless Backend:** Scalable APIs with AWS Lambda and API Gateway.
- **Cloud Storage & CDN:** Asset storage on S3, globally distributed via CloudFront.
- **Containerization:** Dockerized backend for easy local development and cloud deployment.

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- Docker
- AWS Account (for backend services)
- Clerk Account (for authentication)
- Stripe Account (for payments)
- Vercel Account (for frontend deployment)

### Installation

1. **Clone the repository**
```
git clone https://github.com/Marvellousz/Skill-Forge.git
cd Skill-Forge
```

2. **Install dependencies**
```
# Frontend

cd frontend
npm install

# Backend

cd ../backend
npm install
```

3. **Set up environment variables**

Create `.env` files in both `frontend` and `backend` directories. Example variables:

**Frontend**
```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
NEXT_PUBLIC_STRIPE_PUBLIC_KEY=your_stripe_public_key
NEXT_PUBLIC_API_URL=https://your-backend-api-url
```

**Backend**
```
CLERK_SECRET_KEY=your_clerk_secret_key
STRIPE_SECRET_KEY=your_stripe_secret_key
AWS_ACCESS_KEY_ID=your_aws_access_key
AWS_SECRET_ACCESS_KEY=your_aws_secret_key
DYNAMODB_TABLE_NAME=your_table_name
S3_BUCKET_NAME=your_bucket_name
```

4. **Run locally**

- **Frontend**
  ```
  cd frontend
  npm run dev
  ```
- **Backend**
  ```
  cd backend
  npm run dev
  ```

5. **Docker (Backend)**
```
cd backend
docker build -t lms-backend .
docker run -p 5000:5000 lms-backend
```

---

## Architecture Overview

- **Frontend:** Next.js app deployed on Vercel
- **Backend:** Node.js/Express.js APIs on AWS Lambda via API Gateway, containerized with Docker
- **Database:** DynamoDB for fast, scalable NoSQL storage
- **Storage:** AWS S3 for file uploads, distributed via CloudFront
- **Authentication:** Clerk for secure, modern auth flows
- **Payments:** Stripe integration for billing and subscriptions

---

## Project Structure

```
/frontend      \# Next.js app (UI, state, client logic)
/backend       \# Node.js/Express API (business logic, AWS integration)
/diagrams      \# System architecture and data models
/assets        \# Images, icons, and other assets
```


