# fastSocial

## Social Media Backend API

A comprehensive FastAPI implementation replicating the backend functionality of a social media application.

## Features

- **Post Management:** Create, delete, update, and view posts.
- **User Management:** Create user accounts and search for users by ID.
- **Authentication:** Secure login system for user authentication.
- **Voting/Likes:** Upvote and downvote posts to express preferences.

## Local Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/sebwylleman/fastSocial.git 
   cd fastSocial
   ```

2. **Install Dependencies:**

   ```bash
   pip install fastapi
   ```

3. **Set Up Database (PostgreSQL):**

   - Create a PostgreSQL database.
   - Create a `.env` file in the project root directory with the following content:

     ```
     DATABASE_HOSTNAME=localhost
     DATABASE_PORT=5432
     DATABASE_PASSWORD=<your_password>
     DATABASE_NAME=<your_database_name>
     DATABASE_USERNAME=<your_username>
     SECRET_KEY=<your_secret_key>
     ALGORITHM=HS256
     ACCESS_TOKEN_EXPIRE_MINUTES=60
     ```

     Replace placeholders with your actual database credentials and a strong secret key. You can generate a secret key using tools like OpenSSL or secrets module in Python.

4. **Run the Server:**

   ```bash
   uvicorn main:app --reload
   ```

5. **Access the API:**
   Open your browser and navigate to:
   ```
   http://127.0.0.1:8000/docs
   ```

## API Endpoints

The interactive API documentation (Swagger UI) at `http://127.0.0.1:8000/docs` provides a detailed list of available endpoints, their parameters, and expected responses.

## Additional Notes

- This project is a learning exercise and may not be suitable for production use without further modifications and security enhancements.
- Consider exploring additional features like commenting, following/followers, real-time updates, etc., to make the API more comprehensive.
