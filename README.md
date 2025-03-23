Here’s your `README.md` file in a well-structured format:

---

```markdown
# EduLearn: Online Learning & Book Management Platform

EduLearn is a full-stack web application built with the **MERN** (MongoDB, Express.js, React, Node.js) stack. This application allows users to browse books, sign up, log in, and purchase books seamlessly. 

The frontend is built using **React, Vite, and Tailwind CSS**, while the backend leverages **Node.js, Express.js**, and **MongoDB**. User authentication is secured with **bcrypt.js** for password hashing.

---

## 📚 Features

### Frontend
- ✅ User Authentication (Signup, Login, Logout)
- ✅ Responsive UI using Tailwind CSS
- ✅ Dark Mode Support
- ✅ Book Listing and Course Browsing
- ✅ API Integration with Axios
- ✅ Client-side Routing using React Router

### Backend
- 🔐 User Authentication (Signup & Login with Hashed Passwords using bcrypt.js)
- 🗂️ RESTful APIs for Books and Users
- 📡 MongoDB Database Integration with Mongoose
- 🛑 CORS Enabled
- 🔐 Environment Variables using dotenv

---

## ⚙️ Installation & Setup

### Prerequisites
Ensure you have the following installed on your system:
- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [Postman](https://www.postman.com/)

> 💡 **Tip:** Use MongoDB Compass to visually manage your database with ease.

---

## 🚀 Backend Setup

1. Open a terminal and navigate to the `Backend/` directory:
```bash
cd Backend
```

2. Install backend dependencies:
```bash
npm install
```

3. Create a `.env` file and add the following variables:
```bash
PORT=4001
MongoDBURI="mongodb://localhost:27017/edulearn"
```

4. Start the backend server:
```bash
npm start
```

✅ If everything is correct, the terminal should display:
```
Server is listening on port 4001
Connected to mongoDB
```

⚠️ **Warning:** Ensure that MongoDB is running before starting the backend server to avoid connection errors.

---

## 📦 MongoDB Setup

### For Local MongoDB:
1. Open MongoDB Compass or run MongoDB in the terminal:
```bash
mongod
```

2. Create a new database named `edulearn`.

3. Add two collections:
   - `users`
   - `books`

---

## 📚 Sample MongoDB Data

### Users Collection
```json
{
  "fullname": "Ravikant",
  "email": "ravikant@gmail.com",
  "password": "$2a$10$VbUJh1ZrXsE3/jgEmS0SOuO"
}
```

### Books Collection
```json
{
  "name": "Data Structures and Algorithmic Analysis in C++",
  "price": 1599,
  "category": "DSA",
  "image": "images/dsa.jpg",
  "title": "Introduction to Algorithms by Thomas Cormen"
}
```

⚠️ **Important:** Use `bcrypt.js` to store passwords securely before inserting data into MongoDB.

---

## 🧪 Postman API Testing

1. Open Postman.
2. Create a new POST request for user signup:
- **URL:** `http://localhost:4001/user/signup`
- **Body (JSON):**
```json
{
  "fullname": "Ravikant",
  "email": "ravikant@gmail.com",
  "password": "password123"
}
```
3. Click **Send** and verify the response.
4. Similarly, test login and book APIs.

⚠️ **Caution:** Do not share your JWT tokens or API keys publicly to maintain security.

---

## 🎨 Frontend Setup

1. Open a terminal and navigate to the `Frontend/` directory:
```bash
cd Frontend
```

2. Install frontend dependencies:
```bash
npm install
```

3. Start the frontend development server:
```bash
npm run dev
```

4. Open the browser and go to:
```
http://localhost:5173/
```

---

## 📁 Project Structure

```
edulearn-app/
├── Backend/
│   ├── index.js
│   ├── .env
│   ├── controller/
│   │   ├── book.controller.js
│   │   ├── user.controller.js
│   ├── model/
│   │   ├── book.model.js
│   │   ├── user.model.js
│   ├── route/
│   │   ├── book.route.js
│   │   ├── user.route.js
│   ├── package.json
│   ├── package-lock.json
├── Frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── context/
│   │   ├── courses/
│   │   ├── home/
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   ├── index.css
│   ├── tailwind.config.js
│   ├── vite.config.js
│   ├── package.json
│   ├── package-lock.json
│   ├── postcss.config.js
│   ├── .gitignore
│   ├── .eslintrc.cjs
├── README.md
```

---

## 🛠️ Tech Stack

### Frontend
- ⚡ React
- ⚡ Vite
- 🎨 Tailwind CSS

### Backend
- 🚀 Node.js
- 🚀 Express.js

### Database
- 📚 MongoDB

### Authentication
- 🔐 bcrypt.js

### API Testing
- 🧪 Postman

---

## 📝 License
This project is licensed under the MIT License. Feel free to modify and use this project as needed.

---

## 📧 Contact
For any queries or contributions, reach out at [your-email@example.com].
```

---

✅ This `README.md` is clean, organized, and follows best practices for documentation. Let me know if you need any changes! 🚀
