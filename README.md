
# Simple Authentication System with Express and JWT

This repository contains a basic authentication system implemented using Express.js and JSON Web Tokens (JWT). The system allows users to sign in, generates a token upon successful authentication, and provides a route to retrieve a list of users (excluding the authenticated user) using Postman or similar tools.

## Installation

1. **Clone the Repository:**
    ```bash
    git clone https://github.com/Rohitkumar43/Simple-Authentication.git
    ```
    Clone the repository to your local machine using the above command.

2. **Navigate to the Project Directory:**
    ```bash
    cd Simple-Authentication
    ```
    Move into the cloned project directory.

3. **Install Dependencies:**
    ```bash
    npm install
    ```
    Install the necessary Node.js dependencies for the project.

4. **Configuration:**
    - Make sure to configure any environment variables if required. For instance, check and update the JWT secret key (`jwtPassword`) in the codebase as needed.

5. **Start the Server:**
    ```bash
    node app.js
    ```
    Launch the server to begin using the authentication system.

## Usage

1. **Sign In:**
   - **Endpoint:** `POST /signin`
   - **Input:** Provide `username` and `password` in the request body.
   - **Output:** Receives a JWT token upon successful authentication.

   Example Request Body:
   ```json
   {
     "username": "rohitkumar@gmail.com",
     "password": "123"
   }




## Important Notes

This system uses an in-memory database with predefined user data for demonstration purposes. It should be replaced with a proper database in production.
Ensure that the JWT password (jwtPassword) is kept secure. In production, consider using environment variables for sensitive information.
The code logic for user authentication and retrieving user lists is basic and can be enhanced for a production-ready application, incorporating encryption, validation, error handling, etc.

