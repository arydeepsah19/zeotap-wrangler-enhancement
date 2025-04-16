# Zeotap Data Ingestion Assignment

This project demonstrates a basic data ingestion pipeline using Spring Boot for backend ingestion services and a frontend UI to initiate the ingestion process. It simulates ingestion of a flat file (CSV) into ClickHouse through a web interface.

## 🧱 Project Structure

zeotap-assignment/ ├── backend/ # Spring Boot Application │ ├── src/ │ ├── pom.xml │ └── ... ├── frontend/ # React or frontend of your choice │ ├── public/ │ ├── src/ │ ├── package.json │ └── ... └── README.md

yaml
Copy
Edit

---

## ⚙️ Backend Setup (Spring Boot)

### Prerequisites

- Java 17+
- Maven

### Setup Instructions

1. Navigate to backend folder:
   ```bash
   cd backend
Build the project:

bash
Copy
Edit
mvn clean install
Run the Spring Boot application:

bash
Copy
Edit
mvn spring-boot:run
Backend will be available at http://localhost:8081

💻 Frontend Setup
Prerequisites
Node.js (v16+ recommended)

npm or yarn

Setup Instructions
Navigate to frontend folder:

bash
Copy
Edit
cd frontend
Install dependencies:

bash
Copy
Edit
npm install
Run the frontend:

bash
Copy
Edit
npm start
UI will be available at http://localhost:3000

📊 Features
Upload CSV file path via frontend UI.

Send request to backend to ingest the file.

Backend parses file and logs each row (mock ClickHouse insert).

📁 Sample Payload
json
Copy
Edit
{
  "fileName": "mock/path.csv",
  "delimiter": ",",
  "header": true
}
✅ Notes
Replace mock/path.csv with the absolute path to your CSV file on your system.

No real ClickHouse connection — this mock simulates ingestion pipeline only.

📌 Final Deliverables
✅ Full source code checked into GitHub.

✅ README with setup and run instructions (this file).

yaml
Copy
Edit

---

Let me know if you want to tweak this based on your actual frontend tech (React, HTML, etc.) or want to add screenshots, too.
