Setup Instructions
Clone the Repository
To get started, clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/hm07-qa-us.git
Install Dependencies
After cloning, navigate to the project directory and install all required dependencies:

bash
Copy code
npm install
Update Config File
Replace the API URL in config.js with the unique server URL provided after launching the Urban Grocers server. For example:

js
Copy code
const API_URL = 'https://your-server-url.containerhub.tripleten-services.com';
Test Cases
The project includes the following test cases for API endpoints:

GET Requests
Endpoint: /api/v1/kits/1

Test 1: Checks if the status code is 200.
Test 2: Verifies that the response receives a kit.
POST Requests
Endpoint: /api/v1/orders

Test 1: Ensures the response status is 201.
Test 2: Validates the response body creates a shopping cart
PUT Requests
Endpoint: /api/v1/products/7

Test 1: Verifies that the status code is 200 when updating a product.
Test 2: Confirms that the response body contains an object with "ok": true indicating the update was successful.
DELETE Requests
Endpoint: /api/v1/kits/7

Test 1: Ensures the status code is 200 when deleting a product kit.
Test 2: Confirms the product was deleted correctly, with a response body of "ok": true.
Running Tests
To execute the test suite, run the following command in the project directory:

bash
Copy code
npm test
This will run all test files and report the results in the console.

Submission Process
Make sure all tests pass successfully.
Commit your changes and push them to the repository:
bash
Copy code
git add .
git commit -m "Completed API tests for Project 7"
git push origin main
Verify that the automated tests in the GitHub Actions workflow pass without errors.
Submit the link to your GitHub repository for review.
   