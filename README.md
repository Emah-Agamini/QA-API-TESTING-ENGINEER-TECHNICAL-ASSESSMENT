**QA Engineer Technical API Testing Assessment**

This repository contains a Postman collection used for API test automation of the Swagger Petstore user endpoints. It is designed as part of a QA API Testing Technical Assessment.

**Repository:** [https://github.com/Emah-Agamini/QA-API-TESTING-ENGINEER-TECHNICAL-ASSESSMENT](https://github.com/Emah-Agamini/QA-API-TESTING-ENGINEER-TECHNICAL-ASSESSMENT)

**Postman Collection:** Enyata-QA.postman\_collection.json

**Overview**

The test suite validates various CRUD and authentication operations on user data using the Swagger Petstore API.

**API Base URL:**  
 [https://petstore.swagger.io/v2](https://petstore.swagger.io/v2)

**Endpoints Tested**

The following user-related endpoints are included in the collection:

1. POST /user/createWithList  
     Creates multiple users from a list payload.

2. GET /user/{username}  
     Retrieves details of a single user by username.

3. PUT /user/{username}  
     Updates an existing user's data.

4. DELETE /user/{username}  
     Deletes a user by username.

5. GET /user/login  
     Authenticates user credentials.

6. GET /user/logout  
     Logs out the current user session.

7. POST /user/createWithArray  
     Creates users using an array input.

8. POST /user  
     Creates a single user.

**Prerequisites**

* Postman installed (https://www.postman.com/downloads/)

* Node.js (optional, if running via Newman)

* Internet connection to reach [https://petstore.swagger.io/v2](https://petstore.swagger.io/v2)

How to Use the Collection

1. **Clone the Repository**

git clone [https://github.com/Emah-Agamini/QA-API-TESTING-ENGINEER-TECHNICAL-ASSESSMENT.git](https://github.com/Emah-Agamini/QA-API-TESTING-ENGINEER-TECHNICAL-ASSESSMENT.git)  
 cd QA-API-TESTING-ENGINEER-TECHNICAL-ASSESSMENT

2. **Import into Postman**

* Open Postman

* Click “Import”

* Choose Enyata-QA.postman\_collection.json from this repo

* The collection will be available under "Collections" in Postman

3. Run the Collection

**Option 1: Using Postman Runner**

* Open the collection

* Click “Run Collection”

* Run all requests with or without test data

**Option 2: Using Newman CLI (Optional)**

**Install Newman globally:**

npm install \-g newman

**Run collection:**

newman run Enyata-QA.postman\_collection.json

**Test Data**

Test data (usernames, IDs, login credentials) is hardcoded into each request for simplicity. You can parameterize them using Postman environments or data files for scalable testing.

**Tests and Assertions**

Each request includes Postman test scripts that validate:

* HTTP status codes (200, 400, 404, etc.)

* Response schema (basic key validation)

* Successful login/logout behavior

* Proper CRUD behavior (create → retrieve → update → delete)

**Folder Organization (if any)**

**Requests are grouped into logical folders:**

* Create Users

* Retrieve & Update

* Authentication

* Bulk User Operations

**Best Practices Followed**

* RESTful endpoint coverage of all core operations

* Response code validation and assertion scripts

* Independent and chainable tests

* Reusable request bodies

**Contribution**

This repository was developed for Enyata's technical QA api testing assessment. For questions or feedback, feel free to raise an issue.

**License**

This project is open for review and learning purposes and does not carry a commercial license.

**Author**  
[Agamini Emmanuel](https://www.linkedin.com/in/emmanuel-agamini/)
