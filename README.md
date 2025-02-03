
HNG12 Stage 1 - Number Classification API
Project Description
This is a simple RESTful API that accepts a number and returns interesting mathematical properties about it, along with a fun fact fetched from the Numbers API.

Features
Checks if the number is prime.
Checks if the number is a perfect number.
Checks if the number is an Armstrong number.
Determines if the number is odd or even.
Calculates the sum of digits of the number.
Fetches a fun fact from Numbers API.
Technology Stack
Language: PHP
Hosting Platform: InfinityFree (or your hosting provider)
Live API URL
Base URL:

arduino
Copy
Edit
http://hng2-task.free.nf/
API Endpoint
GET /api/classify-number?number={number}
Description: Takes a number as input and returns its mathematical properties and a fun fact.
Example Request:
bash
Copy
Edit
GET http://hng2-task.free.nf/api/classify-number?number=371
Success Response (200 OK):
json
Copy
Edit
{
    "number": 371,
    "is_prime": false,
    "is_perfect": false,
    "properties": ["armstrong", "odd"],
    "digit_sum": 11,
    "fun_fact": "371 is an Armstrong number because 3^3 + 7^3 + 1^3 = 371"
}
Error Response (400 Bad Request):
json
Copy
Edit
{
    "error": true,
    "message": "Invalid number"
}
Setup Instructions (Running Locally)
Clone the repository:
bash
Copy
Edit
git clone https://github.com/Emek1212/hng2-task.git
cd hng2-task
Start a local PHP server:
bash
Copy
Edit
php -S localhost:8000
Test the API in your browser or Postman:
bash
Copy
Edit
http://localhost:8000/api/classify-number?number=371
Deployment
The API is hosted at: http://hng2-task.free.nf/
Expected response time: < 500ms
Backlink
For PHP developers: Hire PHP Developers

