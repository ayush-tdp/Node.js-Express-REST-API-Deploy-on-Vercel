## **🌍 Node.js + Express REST API & Deploy on Vercel**  

🔥 This guide helps you **create a simple REST API** using **Node.js + Express** and **deploy it on Vercel** with just a few steps!  

🚀 **Quick Setup → Build → Deploy** in minutes!  

---

## **✨ Features**  

✅ **Simple & Fast** - Lightweight and optimized API setup  
✅ **RESTful API** - Create, Read, Update, and Delete (CRUD) operations  
✅ **Vercel Hosting** - Free, fast, and easy deployment  
✅ **CORS Enabled** - Works with frontend applications  
✅ **JSON Responses** - Fully structured data output  

---

## **📦 Project Setup**  

### **1️⃣ Install Node.js & Express**  
Run the following command in your terminal:  
```bash
mkdir express-rest-api && cd express-rest-api
npm init -y
npm install express cors
```

### **2️⃣ Create the Server File**  
📝 **Create a file:** `server.js`  
```javascript
const express = require("express");
const cors = require("cors");

const app = express();
app.use(cors());
app.use(express.json());

const PORT = process.env.PORT || 3000;

// Sample Route
app.get("/", (req, res) => {
    res.json({ message: "🚀 Welcome to the Express API!" });
});

// Sample Users Route
app.get("/users", (req, res) => {
    res.json([
        { id: 1, name: "John Doe" },
        { id: 2, name: "Jane Smith" }
    ]);
});

app.listen(PORT, () => {
    console.log(`✅ Server running at http://localhost:${PORT}`);
});
```

---

## **🚀 Running the API Locally**  

### **Start the Server**  
```bash
node server.js
```
✅ Your API is now running at:  
👉 **http://localhost:3000/**  

---

## **🌍 Deploying to Vercel**  

### **1️⃣ Install Vercel CLI**  
```bash
npm install -g vercel
```

### **2️⃣ Login to Vercel**  
```bash
vercel login
```

### **3️⃣ Deploy the API**  
```bash
vercel
```
💡 Follow the on-screen steps, and once deployed, you’ll get a live API URL! 🎉  

✅ **Example Deployed URL:**  
👉 `https://your-vercel-api.vercel.app/`  

---

## **🛠 API Endpoints**  

| Method | Endpoint      | Description               |
|--------|-------------|---------------------------|
| `GET`  | `/`         | Welcome message 🚀       |
| `GET`  | `/users`    | Get a list of users 👥    |

### **📌 Example Request:**  
```bash
curl -X GET "https://your-vercel-api.vercel.app/users"
```

📌 **Response:**  
```json
[
    { "id": 1, "name": "John Doe" },
    { "id": 2, "name": "Jane Smith" }
]
```

---

## **🔗 Use Cases**
📌 **🔄 API for Frontend Apps** – Use this as a backend for React/Vue/Angular apps  
📌 **📝 JSON Data API** – Fetch and display structured data  
📌 **⚡️ Microservices** – Use as a lightweight service for projects  
📌 **📊 Data Fetching** – Connect with databases later  

---

## **👨‍💻 Author**
Made with ❤️ by **[Your Name](https://github.com/your-username)**  

📌 **GitHub:** [https://github.com/your-username](https://github.com/your-username)  
📌 **Website:** [https://yourwebsite.com](https://yourwebsite.com)  

⭐ **If you found this helpful, give it a star!** 🌟🚀  

---
