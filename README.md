🛒 ROBOSHOP-WITH-DOCKER

Roboshop is a microservices-based Ecommerce application containerized with Docker.
This project follows Docker best practices such as using official images, multi-stage builds, and lightweight containers for secure and optimized deployments.

🚀 Features

Microservices: Cart, Catalogue, User, Payment, Shipping, Frontend

Built with official Docker images (Node.js, MongoDB, Redis, MySQL, RabbitMQ, Nginx)

Multi-stage builds → smaller & faster images

Docker Compose → run all services together
🐳 Docker Best Practices Used

✅ Multi-stage builds (Node.js & Java services)

✅ Official base images (node:20-alpine3.21, nginx:alpine, openjdk:17-slim, etc.)

✅ .dockerignore for smaller images

✅ Containers run as non-root users
