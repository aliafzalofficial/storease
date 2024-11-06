ShopEase E-commerce Microservices Platform
Overview
ShopEase is a microservices-based e-commerce platform that enables users to register, browse products, and place orders seamlessly. Each service runs independently in its own Docker container, allowing scalability and efficient resource management.

Services and Technologies Used
User Service

Function: Handles user registration, authentication, and login.
Technologies: Python Flask, PostgreSQL
Product Service

Function: Manages the product catalog, including adding, updating, and retrieving product information.
Technologies: Node.js, MongoDB
Order Service

Function: Manages order creation, payment processing, and tracking.
Technologies: Java Spring Boot, MySQL
Infrastructure and Supporting Tools
Docker & Docker Compose: Containerize each service and manage dependencies with ease.
Nginx: Configured as a reverse proxy to route incoming requests to the appropriate services based on request paths.
GitHub Actions: CI/CD automation for testing and deployment

Running Locally with Docker Compose
Clone the Repository:
git clone <repository-url>
Set Up Environment Variables:
cp .env.example .env
Build and Run Services with Docker Compose:
docker-compose up --build

Access Services:

User Service: http://localhost:5001
Product Service: http://localhost:5002
Order Service: http://localhost:5003

Stopping the Containers:
docker-compose down

Git Workflow and Collaboration:
Branching Strategy:

main: Stable, production-ready code.
develop: Active development.
Pull Requests (PRs):

Each PR should include a meaningful title, description, and link to any related issues.
Code review required before merging to ensure quality and avoid conflicts.

Commit Messages:

Use descriptive commit messages (e.g. "Add enpoints User Service").