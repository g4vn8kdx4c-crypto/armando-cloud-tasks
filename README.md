Armando Cloud Tasks (Serverless To-Do App)

A fully serverless, full-stack application built on AWS using:
    •    S3 – Frontend hosting
    •    API Gateway – RESTful API
    •    Lambda (Python) – Business logic
    •    DynamoDB – NoSQL database for tasks

This project demonstrates real-world cloud engineering skills including API design, Lambda proxy integration, IAM configuration, CORS troubleshooting, and end-to-end deployment.

⸻

🚀 Live Architecture

Frontend (S3 Static Website)
↓
JavaScript fetch()
↓
API Gateway (/tasks)
↓
Lambda Functions
    •    GET /tasks → returns all tasks
    •    POST /tasks → creates a task
    •    DELETE /tasks → deletes a task
↓
DynamoDB (ArmandoTodos table)

⸻

🧱 Project Structure

armando-cloud-tasks/
│
├── README.md
├── frontend/
│     └── index.html
│
└── lambdas/
      ├── get_all_tasks.py
      ├── create_task.py
      └── delete_task.py

🛠 Technologies Used

S3 – Hosts the frontend UI
API Gateway – REST API for /tasks
Lambda (Python) – Serverless backend logic
DynamoDB – NoSQL task storage
IAM – Roles and permissions for secure access
CORS – Enables browser-based frontend requests

⸻

🔥 Key Features
    •    Add new tasks
    •    Fetch all tasks
    •    Delete tasks
    •    Fully serverless — no backend servers needed
    •    Real-time updates via DynamoDB
    •    Scales instantly
    •    Ultra-low cost architecture

⸻

🧪 Testing the API (curl)

GET all tasks:
curl https://your-api-url/dev/tasks

POST create a new task:
curl -X POST -H “Content-Type: application/json” -d ‘{“task”: “Study cloud engineering”}’ https://your-api-url/dev/tasks

DELETE a task:
curl -X DELETE -H “Content-Type: application/json” -d ‘{“id”: “your-task-id”}’ https://your-api-url/dev/tasks
