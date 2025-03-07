Hotel Booking System Project
Overview
This project is a Hotel Booking System consisting of three main components:

Frontend: Built with React and Vite for fast development and optimal performance.
Backend Service 1: Spring Boot with Spring Security and JWT for secure authentication and handling business logic for bookings.
Backend Service 2: Node.js with Express to manage payment processing and interact with the database.
DataBase: MySQL: Relational database to store bookings and payment information.

Features
User Authentication: Secure login using JWT.
Booking Management: Allows users to view, filter, and manage hotel bookings.
Payment Integration: Processes payments and validates them.
Weather Integration: Fetches weather data for the hotel’s location. (API Public OpenWeatherMap)

Installation

1. Frontend (React & Vite):
1/Clone the repository:
git clone <repository-url>
cd <repository-folder>
2/Install dependencies:
npm install
3/Run the development server:
npm run dev
The frontend should now be running at http://localhost:5173.(vite default port)

2. Backend Service 1 (Spring Boot)
1/Clone the repository for Backend Service 1:
git clone <repository-url>
cd <backend-service-1-folder>
2/Open the project in your IDE and configure the application.properties for the database connection and other settings. (we use IntelliJ IDEA Community Edition 2024.3)
3/Build and run the Spring Boot application:
./mvnw spring-boot:run
The backend should now be running at http://localhost:9192.

3. Backend Service 2 (Node.js & Express)
1/Clone the repository for Backend Service 2:
git clone <repository-url>
cd <backend-service-2-folder>
2/Install dependencies:
npm install
3/Run the backend server:
node server.js   or     npm start
The backend should now be running at http://localhost:3001.

API Endpoints  (you can use postman to verify that it works )
example: 
GET /api/bookings:
Description: Retrieves all bookings.
Requires JWT Authorization in the header: Authorization: Bearer <jwt-token>
Response: List of bookings in JSON format.

Troubleshooting
CORS Errors: Ensure that CORS is properly set up on both backend services.
JWT Expiration: If you get an Unauthorized error, ensure the JWT is still valid and has not expired.

Thank You.



