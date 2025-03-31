Overview
This project enhances a basic calculator microservice by adding advanced arithmetic operations and improving error handling. Both the backend (Node.js + Express) and frontend (HTML + JS) were updated.

Step-by-Step Instructions
1. Implement Calculator Logic (Backend)

Technology: Node.js + Express

New API Endpoints Added:
GET /power?num1=x&num2=y → returns x^y
GET /modulo?num1=x&num2=y → returns x % y
GET /sqrt?num1=x → returns √x

Validation Functions:
validateTwoNumbers(req, res) – checks num1 and num2 are present and valid
validateOneNumber(req, res) – checks num1 is present and valid
All functions return JSON-formatted error messages if invalid inputs are detected.

2. Update Front-End Page

Technology: HTML, CSS, and JavaScript
New Features:
Dropdown menu to select operation (including power, modulo, square root)
Real-time error or success result rendering
Clean UI with responsive layout and styling

User Inputs:
num1 (required for all operations)
num2 (optional for square root)
operation (select from 7 options)

3. Run the Server
 Invalid input → Error: Both num1 and num2 must be valid numbers.
