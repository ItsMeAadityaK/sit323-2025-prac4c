This task expands on the calculator microservice developed in Task 4.1P. The aim is to:
- Add advanced arithmetic operations (Option A)
- Improve the microservice’s error handling mechanism (Option B)

The service is built using Node.js and Express, and exposes RESTful API endpoints for both basic and advanced operations.

Basic Operations (from 4.1P)

- Addition
- Subtraction
- Multiplication
- Division

Enhanced Functionality (Task 4.2C)

Option A – Advanced Arithmetic Operations

- Exponentiation
- Square Root
- Modulo

Option B – Improved Error Handling

- Validates presence and correctness of inputs
- Handles:
  - Missing parameters
  - Non-numeric values
  - Division by zero
  - Square root of negative numbers
  - Modulo by zero


Implementation Process:
1. Extended the index.js file

- Used Express.js to create all routes.
- Middleware Numbers checks for missing or invalid inputs for two-parameter endpoints.
- Custom checks implemented for square root and power.

2. Implemented Advanced Endpoints

- Added logic for exponentiation, square root, and modulo.
- All inputs are parsed as floats for accurate calculations.

3. Improved Error Handling

- Clear error messages returned with HTTP status 400.
- All invalid scenarios are handled with descriptive JSON responses.

4. Tested using Postman

- Successful and error cases were tested and validated.
- All endpoints returned correct results and error messages.