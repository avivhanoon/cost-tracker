Team members:
Name: Aviv Hanoon
ID: 213389315
Mobile number: 0507007607
Email: avivhanoon@gmail.com

Name: Yuval Horesh
ID: 318815966
Mobile number: 0527249222
Email: yuvalhoreshfam@gmail.com


Link to the video: 

PROJECT DESCRIPTION:
Cost Manager RESTful Web Services is a Node.js project that provides RESTful APIs to manage cost data. This project is built with Express.js, MongoDB, and Mongoose.


FEATURES:


Add Cost item: you can a new cost to the database 
Get Monthly Report: Retrieve all cost items for a specific user within a specific month and year.
Get User Details: Retrieve user information along with the total cost for a specific user.
Get Developers Info: Retrieve information about the developers who worked on the project.
PROPERTIES:
Node.js
MongoDB Atlas 

INSTALLATION:
Copy the whole code to VSCODE
Install dependencies: npm install
Configure Enviroment Variables: Create a .env file and add you PORT and MONGO_URI
start the server: npm run devStart
run tests: npm test
API ENDPOINTS:
1. Add Cost Item
Method: POST
Endpoint: /api/add
Request Body:
{
  "description": "Groceries",
  "category": "food",
  "userid": "123123",
  "sum": 100
}
Response:
Success: Returns the added cost item.
Error: Returns an error message.
2. Get Monthly Report
Method: GET
Endpoint: /api/report
Query Parameters:
id: User ID
year: Year (e.g., 2025)
month: Month (1-12)
Response:
Success: Returns an array of cost items.
Error: Returns an error message.
3. Get User Details
Method: GET
Endpoint: /api/users/:id
Response:
Success: Returns user details and total costs.
Error: Returns an error message.
4. Get Developers Info
Method: GET
Endpoint: /api/about
Response:
Returns an array with developer details.

PROJECT STRUCTURE:

├── app.js
├── routes
│   ├── costRoutes.js
│   └── userRoutes.js
├── models
│   ├── cost.js
│   └── user.js
├── tests
│   ├── costRoutes.test.js
│   └── userRoutes.test.js
├── config
│   └── database.js
├── .env
├── package.json
└── README.md


DEPENDENCIES:
express: Web framework for Node.js.
mongoose: MongoDB object modeling tool.
dotenv: Load environment variables from a .env file.
jest: Testing framework (development dependency).
supertest: HTTP assertions for testing (development dependency

Install the dependencies:
run in terminal: npm install express mongoose dotenv jest supertest
