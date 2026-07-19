# Forge Fitness Backend

Backend API for the **Forge Fitness** gym website. It handles booking requests submitted from the frontend and stores them in a PostgreSQL database.

---

## Features

- Receive booking requests from the frontend
- Store user data in PostgreSQL
- REST API built with Express.js
- JSON request handling
- CORS enabled for frontend integration
- Error handling and validation

---

## Technologies Used

- Node.js
- Express.js
- PostgreSQL
- pg (Node PostgreSQL Driver)
- CORS
- dotenv

---

## Project Structure

backend/
│── node_modules/
│── package.json
│── package-lock.json
│── server.js
│── .gitignore
│── README.md

---

## Installation

### Clone the repository

```bash
git clone https://github.com/iqrayaqoob1/forge-fitness-backend.git
```

### Move into the project folder

```bash
cd forge-fitness-backend
```

### Install dependencies

```bash
npm install
```

### Create a .env file

```env
DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=your_password
DB_NAME=forgefitness
PORT=3000
```

Replace the values with your PostgreSQL configuration.

---

## Run the Server

```bash
node server.js
```

or

```bash
npm start
```

Server will start on:

```
http://localhost:3000
```

---

## API Endpoint

### POST /book

Stores a new gym booking.

### Request Body

```json
{
  "name": "Iqra",
  "email": "iqra@example.com",
  "interest": "Strength Training"
}
```

### Success Response

```json
{
  "message": "Booking saved successfully"
}
```

---

## Database

PostgreSQL database contains a table named:

```
bookings
```

Example columns:

- id
- name
- email
- interest
- created_at

---

## Frontend Repository

https://github.com/iqrayaqoob1/forge-fitness-frontend

---

## Live Frontend Demo

https://forge-fitness-iqra.netlify.app

---

## Backend Deployment

The backend is currently configured to run locally using Node.js and PostgreSQL.

---

## Future Improvements

- Deploy backend to a cloud platform
- Authentication
- Email confirmation
- Admin Dashboard
- Booking Management
- Input validation enhancements

---

## Author

**Iqra Yaqoob**


---

## License

This project is developed for learning purposes as part of the DecodeLabs Frontend Development Program.
