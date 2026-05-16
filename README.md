# Dmoney API Integration Testing

## Overview
`Dmoney_API_Integration_Testing` is an API integration testing project for validating the end-to-end transaction flow of the Dmoney system.

This project uses **Postman** for API test design and **Newman** for command-line execution. The main goal is to verify that user creation, user activation, deposit, send money, and cashout transactions work correctly across different roles.

## Test Scenario
The following business flow is automated in this collection:

1. Create 2 customers and 1 agent
2. Activate the created users using Admin API
3. Deposit 5000 tk from System account to Agent account
4. Agent deposits 2000 tk to Customer 1
5. Customer 1 sends 1000 tk to Customer 2
6. Customer 2 cashes out 500 tk from Agent

## Tools & Technologies
- Postman
- Newman
- JavaScript
- GitHub

## Key Validations
- API response status code validation
- User creation validation
- User activation validation
- Transaction success validation
- Dynamic data handling using Postman variables
- Token-based authentication validation
- End-to-end transaction flow verification

## How to Run
Follow the steps below to run this API integration test project locally.

### 1. Clone the Repository

```bash
git clone https://github.com/salminleon/Dmoney_API_Integration_Testing.git
```

### 2. Go to the Project Directory

```bash
cd Dmoney_API_Integration_Testing
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Run the Test Collection

```bash
npm test
```

### 5. Run Collection with Newman Directly

```bash
newman run Dmoney_API_Integration_Testing.postman_collection.json
```

### 6. Generate Newman Report

```bash
newman run Dmoney_API_Integration_Testing.postman_collection.json -r cli,htmlextra
```

### 7. View Test Report

After execution, open the generated Newman HTML report from the report folder to review the test results.

## Newman Report
After running the collection, Newman can generate a report to review the test execution result, including passed and failed test cases.

## Project Purpose
This project demonstrates a real-world API integration testing approach from an SDET perspective, focusing on:

- End-to-end API workflow validation
- Role-based transaction flow testing
- Reusable and maintainable test collection
- Automated test execution using Newman
- Professional API testing practice

## Author
**Salmin Leon**  
SDET | API Testing | Postman | Newman | Automation Testing


## API Documentation
[Click here to see API documentation](https://documenter.getpostman.com/view/54839830/2sBXqQHJQi)


#Output
Newman report
<img width="554" height="578" alt="image" src="https://github.com/user-attachments/assets/4446d256-29bb-453a-a5d1-fb872f4590dd" />




