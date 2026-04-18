# Social Media Platform

A full-stack social media application platform built with a Node.js/Express backend and a vanilla HTML/CSS/JS frontend. This project includes user authentication, profiles, and feeds.


## Screenshots : 


![alt text](<Frontend/images/Screenshot 2026-04-18 224327.png>)


![alt text](<Frontend/images/Screenshot 2026-04-18 224310.png>)


![alt text](<Frontend/images/Screenshot 2026-04-18 224255.png>)


## 📂 Folder Structure

```text
Social_media/
│
├── Backend/                 # Express API server
│   ├── middleware/          # Custom middlewares (e.g., Auth protection)
│   ├── models/              # Mongoose database models
│   ├── routes/              # Express API endpoints
│   ├── .env                 # Environment variables (Create this file!)
│   ├── package.json         # Backend dependencies
│   └── server.js            # Entry point for the server
│
├── Frontend/                # Client-Facing Interface
│   ├── css/                 # Stylesheets for the UI
│   ├── js/                  # Client-side JavaScript logic
│   ├── auth.html            # Login/Signup page
│   ├── index.html           # Main social feed
│   └── profile.html         # User profile page
│
└── README.md                # Project documentation
```

---

## 💻 How to Run Locally

To get the project running locally, you need to start the **Backend** and the **Frontend** separately. 

### Prerequisites

- [Node.js](https://nodejs.org/) installed on your machine.
- A [MongoDB](https://www.mongodb.com/) URI string (local or Atlas) to connect the database.

---

### Step 1: Run the Backend

1. Navigate to the `Backend` directory:
   ```bash
   cd Backend
   ```
2. Install the backend dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `Backend/` folder with the necessary environment variables:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```
4. Start the server:
   ```bash
   npm start
   ```
   *The backend should now be running on http://localhost:5000 (or the port you specified).*

---

### Step 2: Run the Frontend

Since the frontend is built using standard Vanilla HTML, CSS, and JS, there is no need for a build step or package manager.

1. Navigate to the `Frontend` directory in your file explorer.
2. Directly open `index.html` in your web browser. 
3. *Recommended*: Use an extension like **Live Server** in VS Code to run the frontend locally, avoiding any CORS issues that sometimes happen with `file://` protocols.

## 🛠️ Technology Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Backend:** Node.js, Express.js
- **Database:** MongoDB & Mongoose
- **Authentication:** JSON Web Tokens (JWT), bcryptjs
