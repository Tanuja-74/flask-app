# 🚀 Flask + Express Microservices App (AWS EC2 Deployment)

## 📌 Overview

This project demonstrates the deployment of a microservices-based application using **Flask (Python)** as the frontend and **Express (Node.js)** as the backend on a single EC2 instance.

The application allows users to submit form data, which is processed by the backend API and stored/handled accordingly.

---

## 🧠 Architecture

```
User (Browser)
      ↓
Flask Frontend (Port 5000)
      ↓
Express Backend API (Port 3000)
      ↓
Data Processing
```

---

## ⚙️ Tech Stack

* **Frontend:** Flask (Python)
* **Backend:** Express.js (Node.js)
* **Cloud:** Amazon EC2
* **Communication:** REST API (HTTP)
* **Tools:** Git, npm, pip

---

## 🌐 Features

* User-friendly form interface
* Backend API integration
* Microservices architecture
* Real-time data submission
* Deployed on cloud (EC2)

---

## 📂 Project Structure

```
flask-app/
│
├── backend-express/
│   ├── server.js
│   └── package.json
│
├── frontend-flask/
│   ├── app.py
│   └── templates/
│
└── README.md
```

---

## 🚀 How to Run Locally

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/flask-app.git
cd flask-app
```

---

### 2️⃣ Setup Backend (Express)

```
cd backend-express
npm install
node server.js
```

---

### 3️⃣ Setup Frontend (Flask)

```
cd ../frontend-flask
pip install flask requests
python app.py
```

---

## 🔗 Application URLs

* **Frontend (Flask):** http://localhost:5000
* **Backend (Express):** http://localhost:3000

---

## ☁️ AWS EC2 Deployment Steps

1. Launch EC2 instance on Amazon Web Services
2. Configure security group (Ports: 22, 3000, 5000)
3. Install dependencies:

   * Python3
   * Node.js
   * Git
4. Clone repository on EC2
5. Install project dependencies
6. Run both services on different ports
7. Access via public IP

---

## 🔄 API Integration

Flask communicates with Express using:

```
http://localhost:3000/users
```

* Sends form data via POST request
* Backend processes and returns response

---

## ⚠️ Important Notes

* Ensure both services are running simultaneously
* Use `0.0.0.0` for external access on EC2
* Use `localhost` for internal communication
* Open required ports in security group

---

## 📈 Future Improvements

* Add database integration (MongoDB/MySQL)
* Use Nginx for reverse proxy
* Dockerize the application
* Implement authentication
* Deploy using CI/CD pipeline

---

## 👩‍💻 Author

**Tanuja Kurane**

---

## 🎉 Conclusion

This project successfully demonstrates deploying and integrating two different technologies (Flask & Express) on a single EC2 instance, following a microservices approach.

---
