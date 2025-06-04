Step By Steps Required to Complete or To Run This Project
Tools Required:
•	VS Code - Code editor
•	Node.js & npm - Backend runtime & package manager
•	MongoDB - Database (Local or Atlas)
•	MongoDB Compass (optional but recommended) - GUI for database
•	Live Server (VS Code extension) - To run frontend locally
•	Postman (optional) - API testing
 Project Setup Instructions (Step-by-Step)
Step 1: Backend Setup
•	Open terminal or VS Code terminal
•	Navigate to or create your backend folder:
o	mkdir pos-backend && cd pos-backend
•	Initialize the project:
o	npm init -y
•	Install necessary backend dependencies:
o	npm install express mongoose cors dotenv
•	Install development tools:
o	npm install -D nodemon
•	Create .env file in backend root and add:
o	MONGO_URI=mongodb://localhost:27017/posdb
•	Run backend:
o	npm run dev
After run the above command it shows like this -> MongoDB Connected and Server running on port 5000
Step 2: Frontend Setup
•	Open your frontend folder in VS Code
•	Install the Live Server extension in VS Code
•	Right-click admin.html or pos.html → Open with Live Server
o	Browser will open at:
o	http://127.0.0.1:5500/pos.html
Step 3: Connect Backend to Frontend
•	Frontend script.js should make fetch() calls to:
o	http://localhost:5000/api/products
•	Ensure backend is running at the same time for this to work.

Step 4: Testing
•	Use MongoDB Compass
o	Open MongoDB Compass
o	Connect to: mongodb://localhost:27017
o	Navigate to posdb > products to view data
•	Use Browser
o	http://localhost:5000/api/products
