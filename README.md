# hospital-management-system

## Setup Instructions

### Backend
1. Create a file named `application.properties` from `application-template.properties`.
2. Set the following environment variables:
   - `MONGO_URI`
   - `JWT_SECRET`
   - `ADMIN_PASSWORD`

### Frontend
1. Create a `.env` file using `.env.example`.
2. Set the required environment variables such as `REACT_APP_API_URL`.

### Running the Project
- Use the following commands to run the backend and frontend services:
  - For backend: `./mvnw spring-boot:run`
  - For frontend: `npm start` or `yarn start`.
Medilink DS(3Y1S) project
