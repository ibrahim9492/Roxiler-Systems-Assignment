⭐ Store Rating App

A full-stack web app for users to rate stores, with role-based access:

Admin: manage stores and users

Normal User: browse stores, submit/edit ratings

Store Owner: view ratings and averages for their store

Built with TypeScript (frontend) and Express.js (backend) using PostgreSQL/MySQL.

🚀 Features

User registration & login (JWT auth)

Role-based authorization

Store listing & search

Submit & edit ratings

Store owner dashboard

Admin dashboard

Responsive UI

RESTful API

🛠 Tech Stack

Frontend: TypeScript, Axios, React Router, [CSS framework of choice]

Backend: Node.js, Express.js, bcryptjs, jsonwebtoken

Database: PostgreSQL / MySQL

🗄 Database Schema Users

Field Type Note

id int PK User ID

name string

email string unique

password string hashed

address string

role enum ADMIN / USER / STORE_OWNER

Stores

Field Type Note

id int PK

name string

email string

address string

Ratings

Field Type Note

id int PK

user_id int FK references users(id)

store_id int FK references stores(id)

rating int 1-5 stars

⚙️ Running Locally Clone the repo:

git clone https://github.com/ibrahim9492/Roxiler-Systems-Assignment.git

cd Roxiler-Systems-Assignment

Backend

cd backend

npm install

npm start

Frontend

cd frontend

npm install

npm run dev

📚 API Endpoints (Examples)

Method Endpoint Role

POST /api/auth/register Public

POST /api/auth/login Public

GET /api/stores All users

POST /api/ratings Normal User

PUT /api/ratings/:id Normal User

GET /api/owner/ratings Store Owner

GET /api/owner/average-rating Store Owner

POST /api/admin/stores Admin

POST /api/admin/users Admin

🤝 Contributing

Pull requests are welcome. Please open an issue first to discuss changes.

🙌 Author

[Ibrahim Shaik] — [ibrahimkhalandar02@gmail.com]

GitHub: https://github.com/ibrahim9492