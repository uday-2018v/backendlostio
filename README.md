project/
│
├── models/
│   └── User.js          # User schema (Mongoose)
│
├── routes/
│   └── authRoutes.js    # Login & Signup APIs
│
├── .env                 # Environment variables
├── .gitignore
├── package.json
├── server.js            # Main server file




⚙️ Tech Stack

Node.js

Express.js

MongoDB

Mongoose

JWT (JSON Web Token)

bcryptjs

dotenv

🔌 Database Connection (Mongoose)

MongoDB is connected using Mongoose in server.js.mongoose.connect(process.env.MONGO_URI)


👤 User Model (Schema)

Name

Email

Password (hashed)

Created At

Implemented using Mongoose Schema inside models/User.js.

🔐 Authentication APIs
✅ Signup API

Creates a new user

Hashes password

Generates JWT token

Endpoint

POST /api/signup

✅ Login API

Validates user credentials

Compares password

Generates JWT token

Endpoint

POST /api/login

🔑 Token Generation

JWT token is generated on successful login & signup

Token contains user ID

Used for authentication in protected routes

🌱 Environment Variables (.env)

Create a .env file in root directory:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

▶️ How to Run the Project

1️⃣ Install dependencies

npm install


2️⃣ Start server

npm start


or

node server.js

📌 API Testing

You can test APIs using:

Postman

Thunder Client

cURL

✅ Status

✔ MongoDB connected
✔ User schema added
✔ Login API created
✔ Signup API created
✔ JWT token generation implemented

👨‍💻 Author

Udayveer Singh
Backend Developer | Node.js | MongoDB

