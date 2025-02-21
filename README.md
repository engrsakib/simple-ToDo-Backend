### TaskStorm Backend - README  

# TaskStorm Backend  

## 🔹 Short Description  
TaskStorm is a full-stack task management application where users can add, edit, delete, and reorder tasks using a drag-and-drop interface. The backend is built with Express.js, MongoDB, and other essential dependencies to manage tasks in real-time while ensuring data persistence.  

## 🔹 Live Links  
- **Frontend Live:** [TaskStorm Live](https://engrsakib-todo-applications.surge.sh/)  
- **Backend Repository:** [GitHub - Backend](https://github.com/engrsakib/simple-ToDo-Backend)  
- **Frontend Repository:** [GitHub - Frontend](https://github.com/engrsakib/simple-ToDo-frontend)  
- **Website:** [Md. Nazmus Sakib](https://www.engrsakib.com/)  
- **Contact:** info@engrsakib.com  

## 🔹 Technologies Used  
- **Backend:** Node.js, Express.js, MongoDB  
- **Authentication:** JSON Web Token (JWT)  
- **Environment Management:** Dotenv  
- **Database Management:** MongoDB  
- **Time Management:** Moment-Timezone  
- **Security & Middleware:** CORS, Cookie-Parser  

## 🔹 Dependencies  
- axios  
- cookie-parser  
- cors  
- dotenv  
- express  
- jsonwebtoken  
- moment-timezone  
- mongodb  

## 🔹 Installation Steps  
Follow these steps to set up and run the backend server:  

1️⃣ **Clone the repository**  
```bash
git clone https://github.com/engrsakib/simple-ToDo-Backend.git
cd simple-ToDo-Backend
```  

2️⃣ **Install dependencies**  
```bash
npm install
```  

3️⃣ **Set up environment variables**  
Create a `.env` file in the root directory and add:  
```
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```  

4️⃣ **Run the server**  
```bash
npm start
```  

5️⃣ **Server will run on**  
```
http://localhost:5000
```  

This backend supports CRUD operations for task management and real-time updates through API endpoints. 🚀  