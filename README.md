# Armando Cloud Tasks

A **full-stack, fully serverless task management application** built on AWS. This project demonstrates real-world cloud engineering skills by combining a public frontend with a production REST API and persistent storage.

---

## 🔗 Live Demo

* **Frontend (S3 Static Website):**
  [http://armando-static-website.s3-website-us-west-1.amazonaws.com](http://armando-static-website.s3-website-us-west-1.amazonaws.com)

* **API Endpoint (API Gateway):**
  [https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks](https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks)

---

## 🏗 Architecture Overview

**Browser** → **S3 Static Website** → **API Gateway (REST)** → **AWS Lambda (Python)** → **DynamoDB**

* Frontend makes `fetch()` calls to the REST API
* API Gateway routes requests to Lambda using proxy integration
* Lambda performs CRUD operations on DynamoDB
* CORS enabled for browser access

---

## ✨ Features

* View all tasks
* Add a new task
* Delete an existing task
* Fully serverless (no servers to manage)
* Persistent storage with DynamoDB
* Scales automatically
* Ultra low-cost AWS architecture

---

## 🧱 Tech Stack

* **Amazon S3** — Static frontend hosting
* **Amazon API Gateway** — REST API
* **AWS Lambda (Python 3.10)** — Backend logic
* **Amazon DynamoDB** — NoSQL database
* **IAM** — Fine-grained permissions per Lambda function
* **CORS** — Browser-based API access

---

## 📂 Project Structure

```
armando-cloud-tasks/
├── README.md
├── frontend/
│   └── index.html
└── lambdas/
    ├── get_all_tasks.py
    ├── create_task.py
    └── delete_task.py
```

---

## 🧪 API Usage Examples

### Get all tasks

```bash
curl https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks
```

### Create a task

```bash
curl -X POST -H "Content-Type: application/json" \
-d '{"task":"Study cloud engineering"}' \
https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks
```

### Delete a task

```bash
curl -X DELETE -H "Content-Type: application/json" \
-d '{"id":"TASK_ID_HERE"}' \
https://ja88qghpxd.execute-api.us-west-1.amazonaws.com/dev/tasks
```

---

## 🧠 What I Learned

* Designing REST APIs with API Gateway
* Lambda proxy integration
* IAM least-privilege role design
* DynamoDB data modeling
* CORS troubleshooting
* End-to-end AWS deployment
* Connecting frontend applications to cloud APIs

---

## 🚀 Future Improvements

* CI/CD with CodeBuild and CodePipeline
* CloudWatch logging and alarms
* Authentication (Cognito)
* Pagination for large datasets

---

## 👤 Author

**Armando Cortez**
Aspiring Cloud Engineer | AWS | Serverless Architecture
