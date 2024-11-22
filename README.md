Real Estate Web Application
A MERN stack web app for real estate listings, including user authentication, property management, and real-time updates using WebSocket.

Technologies Used
Frontend: React, Material UI
Backend: Node.js, Express.js, Prisma ORM
Database: MongoDB
Real-Time Communication: WebSocket
Containerization: Docker
CI/CD: Azure Pipelines
Features
User authentication (registration, login, profile)
Create, edit, and delete property listings
Real-time property updates and chat
Admin dashboard for managing listings and users
Installation
Clone the repository and navigate to the project directory.

Install dependencies:

Backend: cd api && npm install
Frontend: cd client && npm install
Set up environment variables in .env (MongoDB URI, JWT secret, etc.).

Running Locally
Start the Backend: cd api && npm run dev
Start the Frontend: cd client && npm start
Docker (Optional)
If you prefer to use Docker for containerization, you can build and run the app in containers: docker-compose up --build

Testing
To run the tests: npm run test

CI/CD
The project is integrated with Azure Pipelines for automatic builds and deployments.

License
MIT License
