// Project: RehabConnect (MongoDB Version)
// Stack: Node.js + Express + Mongoose (MongoDB)

// File: README.md

# RehabConnect Backend – Node.js + MongoDB

A RESTful backend API for logging and tracking physical therapy sessions.
This version uses Node.js with Express and MongoDB (via Mongoose).

---

## Features
- REST API: POST /log, GET /progress/:patientId
- MongoDB schema for rehab sessions
- JSON-based communication
- Cleanly separated routes, models, and controllers

---

## Tech Stack
- Node.js
- Express.js
- MongoDB + Mongoose
- Nodemon (for dev reloads)
- dotenv (env variable config)

---

## Endpoints
| Method | Route                     | Description                         |
|--------|---------------------------|-------------------------------------|
| POST   | `/log`                    | Log a new rehab session             |
| GET    | `/progress/:patientId`   | Get all sessions for a patient      |

---

## Folder Structure
```
rehabconnect-backend-mongodb/
├── models/
│   └── SessionLog.js
├── routes/
│   └── sessionRoutes.js
├── controllers/
│   └── sessionController.js
├── .env
├── app.js
├── package.json
└── README.md
```

---

## Setup Instructions

```bash
git clone https://github.com/yourusername/rehabconnect-backend-mongodb.git
cd rehabconnect-backend-mongodb
npm install
cp .env.example .env # Then fill in your Mongo URI
npm run dev
```

---

## Example Mongo Document
```json
{
  "patientId": "abc-123",
  "sessionDate": "2025-07-14",
  "painLevel": 3,
  "exercises": ["Bridge", "Bird Dog"],
  "repsCompleted": 25
}
```

---

## License
MIT
