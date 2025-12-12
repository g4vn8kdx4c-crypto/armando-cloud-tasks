# Armando Cloud Tasks

A **full-stack, fully serverless task management application** built on AWS.  
This project demonstrates real-world cloud engineering skills by combining a public frontend with a production REST API and persistent storage.

---

## 🔗 Live Demo

- **Frontend (S3 Static Website):**  
  http://armando-static-website.s3-website-us-west-1.amazonaws.com

- **API Endpoint (API Gateway):**  
  https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks

---

## 🏗 Architecture Overview

**Browser**  
→ **S3 Static Website**  
→ **API Gateway (REST)**  
→ **AWS Lambda (Python)**  
→ **DynamoDB**

- Frontend uses JavaScript `fetch()` to call the REST API  
- API Gateway routes requests using Lambda proxy integration  
- Lambda performs CRUD operations on DynamoDB  
- CORS enabled for browser-based access  

---

## ✨ Features

- View all tasks  
- Add new tasks  
- Delete existing tasks  
- Fully serverless (no servers to manage)  
- Persistent storage with DynamoDB  
- Scales automatically  
- Ultra low-cost AWS architecture  

---

## 🧱 Tech Stack

- **Amazon S3** — Static frontend hosting  
- **Amazon API Gateway** — REST API  
- **AWS Lambda (Python 3.10)** — Backend logic  
- **Amazon DynamoDB** — NoSQL database  
- **IAM** — Fine-grained permissions per Lambda function  
- **CORS** — Secure browser-to-API communication  

---

## 📂 Project Structure# Armando Cloud Tasks

A **full-stack, fully serverless task management application** built on AWS.  
This project demonstrates real-world cloud engineering skills by combining a public frontend with a production REST API and persistent storage.

---

## 🔗 Live Demo

- **Frontend (S3 Static Website):**  
  http://armando-static-website.s3-website-us-west-1.amazonaws.com

- **API Endpoint (API Gateway):**  
  https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks

---

## 🏗 Architecture Overview

**Browser**  
→ **S3 Static Website**  
→ **API Gateway (REST)**  
→ **AWS Lambda (Python)**  
→ **DynamoDB**

- Frontend uses JavaScript `fetch()` to call the REST API  
- API Gateway routes requests using Lambda proxy integration  
- Lambda performs CRUD operations on DynamoDB  
- CORS enabled for browser-based access  

---

## ✨ Features

- View all tasks  
- Add new tasks  
- Delete existing tasks  
- Fully serverless (no servers to manage)  
- Persistent storage with DynamoDB  
- Scales automatically  
- Ultra low-cost AWS architecture  

---

## 🧱 Tech Stack

- **Amazon S3** — Static frontend hosting  
- **Amazon API Gateway** — REST API  
- **AWS Lambda (Python 3.10)** — Backend logic  
- **Amazon DynamoDB** — NoSQL database  
- **IAM** — Fine-grained permissions per Lambda function  
- **CORS** — Secure browser-to-API communication  

---

## 📂 Project Structurearmando-cloud-tasks/
├── README.md
├── frontend/
│   └── index.html
└── lambdas/
├── get_all_tasks.py
├── create_task.py
└── delete_task.py

## 🧪 API Usage Examples

### Get all tasks
```bashcurl -X POST -H "Content-Type: application/json" \
-d '{"task":"Study cloud engineering"}' \curl -X DELETE -H "Content-Type: application/json" \
-d '{"id":"TASK_ID_HERE"}' \
https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/taskshttps://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/taskscurl https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks
