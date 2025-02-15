# **📚 Book Sharing | Pair-Programming-Hackathon-CourseVita**  
A **peer-to-peer book-sharing platform** built for the **Pair Programming Hackathon (CourseVita)**.  
Users can **list, find, exchange, and chat** with nearby book owners!  


---

## **🌍 Live Demo**

![image](https://github.com/user-attachments/assets/013b104f-0037-4755-bbc9-6bf8e2f79f4c)

![image](https://github.com/user-attachments/assets/ddc534f9-28dc-435c-80e7-22df7c457d7e)

![image](https://github.com/user-attachments/assets/04f70c0d-12c2-4a46-a84b-9a6e56daf912)


---

## **🚀 About**  
📚 **Book Sharing** is a **web & mobile platform** where users can **lend out** or **give away books for free**.  

✅ **Key Features:**  
✔️ **User Authentication**: Register/Login via **Email & Google OAuth**  
✔️ **Book Listings**: Users can **post books** for lending or giving away  
✔️ **Book Search**: Search books via **Goodreads API** (title, author, ratings)  
✔️ **Google Maps API**: 📍 **Find books near you** using **Geolocation API**  
✔️ **In-App Chat**: Users can **chat before exchanging books**  
✔️ **Exchange Requests**: Users can **send & accept book requests**  
✔️ **History & Reviews**: Rate and review users after exchanges  

---

## **📌 User Instructions**
📌 **Create an account** (Email & Password or Google Login)  
📌 **List a book** with details (**title, author, condition, location**)  
📌 **Find books near you** via **Google Maps API**  
📌 **Request a book**, chat with the owner, and exchange!  
📌 **Rate & review** the user after exchange  

---

## **🛠️ Tech Stack**
| Layer      | Technology   |
|------------|-------------|
| **Frontend**   | React.js, Redux, Material UI |
| **Backend**    | Node.js, Express.js |
| **Database**   | MongoDB (Mongoose ORM) |
| **Authentication** | JWT, Google OAuth |
| **APIs** | Google Maps API, Goodreads API |
| **Messaging** | Socket.io for real-time chat |
| **Search** | Algolia for full-text search |
| **Deployment** | Firebase (Hosting), Vercel (Frontend), Render (Backend) |

---

## **📂 Project Structure**
This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).  

```
📦 book-sharing
 ┣ 📂 backend
 ┃ ┣ 📂 models
 ┃ ┃ ┣ 📜 User.js
 ┃ ┃ ┣ 📜 Book.js
 ┃ ┣ 📂 routes
 ┃ ┃ ┣ 📜 auth.js
 ┃ ┃ ┣ 📜 books.js
 ┃ ┃ ┣ 📜 chat.js
 ┃ ┣ 📜 server.js
 ┃ ┣ 📜 .env
 ┃ ┣ 📜 package.json
 ┣ 📂 frontend
 ┃ ┣ 📂 src
 ┃ ┃ ┣ 📂 components
 ┃ ┃ ┃ ┣ 📜 BookList.js
 ┃ ┃ ┃ ┣ 📜 Chat.js
 ┃ ┃ ┃ ┣ 📜 MapComponent.js
 ┃ ┃ ┣ 📂 pages
 ┃ ┃ ┃ ┣ 📜 Register.js
 ┃ ┃ ┃ ┣ 📜 Login.js
 ┃ ┃ ┣ 📜 App.js
 ┃ ┃ ┣ 📜 index.js
 ┃ ┣ 📜 package.json
 ┣ 📜 README.md
```

---

## **📜 Setup Instructions**
### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/RahulDasari1/Book-Sharing.git
cd book-sharing
```

### **2️⃣ Backend Setup**
```bash
cd backend
npm install
```
Create a `.env` file in `backend/`:
```
MONGO_URI = your_mongodb_connection_string
JWT_SECRET = your_jwt_secret
```
Start the backend:
```bash
node server.js
```

### **3️⃣ Frontend Setup**
```bash
cd frontend
npm install
```
Update **Google Maps API Key** in `src/components/MapComponent.js`:
```js
<LoadScript googleMapsApiKey="YOUR_GOOGLE_MAPS_API_KEY">
```
Start the frontend:
```bash
npm start
```

---

## **📡 Deployment**
### **🚀 Deploy Backend to Render**
1. Create a **[Render](https://render.com/)** account.
2. Click **New Web Service** → **Connect GitHub Repo** or **Upload Code**.
3. Add environment variables in **Render dashboard**:
   ```
   MONGO_URI = your_mongodb_connection_string
   JWT_SECRET = your_jwt_secret
   ```
4. Deploy & get backend URL (e.g., `https://book-sharing-backend.onrender.com`).

### **🚀 Deploy Frontend to Firebase/Vercel**
1. Install **Firebase CLI**:
   ```bash
   npm install -g firebase-tools
   ```
2. Deploy:
   ```bash
   firebase login
   firebase init
   firebase deploy
   ```
3. Get frontend URL (e.g., `https://book-sharing.firebaseapp.com`).

---

## **📝 API Endpoints**
### **User Authentication**
| Method | Endpoint | Description |
|--------|----------|------------|
| POST   | `/auth/register` | Register new user |
| POST   | `/auth/login` | Login user |

### **Book Management**
| Method | Endpoint | Description |
|--------|----------|------------|
| POST   | `/books/add` | Add a new book |
| GET    | `/books/nearby?lat={latitude}&lng={longitude}` | Get books nearby |

---

## **📜 Pages**
✔ **Sign in/up Page**  
✔ **Forgot Password Page**  
✔ **Book Overview Page**  
✔ **Book Detail Page**  
✔ **Add Book Page**  
✔ **Requests/History Page**  
✔ **Account Page** (Edit Profile, Upload Avatar, Change Password)  

---

## **🎨 Screenshots**
| Home Page | Chat System |
|-----------|------------|
| ![Home Page](https://via.placeholder.com/400) | ![Chat System](https://via.placeholder.com/400) |

---

## **👨‍💻 Contributing**
🙌 Contributions are welcome!  
1. **Fork the repo**  
2. **Create a feature branch** (`git checkout -b feature-name`)  
3. **Commit changes** (`git commit -m "Added feature XYZ"`)  
4. **Push to GitHub** (`git push origin feature-name`)  
5. **Create a Pull Request**  

---

## **🛡️ License**
📜 MIT License – Free to use & modify.  

---

## **📞 Contact**
📧 **Email:** [dasarirahulpatel.drp@gmail.com](mailto:dasarirahulpatel.drp@gmail.com)  
👔 **LinkedIn:** [Rahul Dasari](https://www.linkedin.com/in/rahul-dasari-drp/)  
🐙 **GitHub:** [RahulDasari1](https://github.com/RahulDasari1)  

---

🚀 **Live Demo:** [https://book-sharing.firebaseapp.com](https://book-sharing.firebaseapp.com)  

---

🎉 **This README is tailored for the** _Pair Programming Hackathon (CourseVita)_.   
Would you like help setting up **Redux for state management or Firebase Authentication**? 😊
