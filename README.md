📚 Book API - Node.js + Express

A simple REST API for managing books (CRUD operations) built with Node.js and Express.  
Data is stored **in-memory** (no database) for demonstration purposes.

---

## 🚀 Features
- **GET** `/books` → Get all books
- **GET** `/books/:id` → Get a book by ID
- **POST** `/books` → Add a new book
- **PUT** `/books/:id` → Update a book by ID
- **DELETE** `/books/:id` → Remove a book by ID

---

## 📦 Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/book-api.git
2. Navigate to the project folder:

bash
cd book-api

3.Install dependencies:

bash
npm install

4.(Optional) Install nodemon for auto-restart:

bash
npm install --save-dev nodemon



▶️ Running the Server
For normal run:

bash
node server.js

For auto-restart with nodemon:

bash
npx nodemon server.js


Server will start at:

arduino
http://localhost:3000



🛠 API Endpoints
1. Get all books
GET http://localhost:3000/books

Response:

json
[
  { "id": 1, "title": "The Alchemist", "author": "Paulo Coelho" },
  { "id": 2, "title": "Atomic Habits", "author": "James Clear" }
]


2. Get a single book
GET http://localhost:3000/books/1

3. Add a book
POST http://localhost:3000/books

Body (JSON):

json
{ "title": "New Book", "author": "John Doe" }


4. Update a book
PUT http://localhost:3000/books/1

Body (JSON):

json
{ "title": "Updated Title", "author": "Updated Author" }


5. Delete a book
DELETE http://localhost:3000/books/1

