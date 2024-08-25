

---

# A Modern AI Chatbot

This project is a modern AI chatbot that leverages the OpenAI API to create an intelligent assistant. The application stores users' chat history in a MongoDB database, allowing users to track conversations and delete them anytime.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Environment Variables](#environment-variables)
- [API Endpoints](#api-endpoints)
- [License](#license)

## Installation

### Prerequisites

- [Node.js](https://nodejs.org/en/) (v14 or above)
- [MongoDB](https://www.mongodb.com/try/download/community) (for local development)
- [pnpm](https://pnpm.io/) (Package manager)

### Backend

1. Clone the repository:
    ```bash
    git clone https://github.com/RkanGen/MERN_Ai_Chat_bot.git
    cd MERN_Ai_Chat_bot/backend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Set up environment variables by creating a `.env` file in the `backend` directory:
    ```bash
    touch .env
    ```

4. Add the following environment variables:
    ```
    MONGO_URI=mongodb://localhost:27017/yourdbname
    OPENAI_API_KEY=your-openai-api-key
    JWT_token=*****
    
    ```

5. Run the backend server:
    ```bash
    npm run dev
    ```

### Frontend

1. Navigate to the frontend directory:
    ```bash
    cd ../frontend
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

3. Start the frontend development server:
    ```bash
    npm run dev
    ```
![image](https://github.com/user-attachments/assets/974b75cc-bc99-42b7-a690-36075dcd25d5)
![merngpt](https://github.com/user-attachments/assets/eaa456cf-445b-48af-a055-422b8d3abdf5)

## Usage

- Open your browser and navigate to `http://localhost:5187` to access the frontend.
- The backend server will be running on `http://localhost:5000`.

## Project Structure

### Backend

- **src/config**: Contains configuration files for the backend.
- **src/controllers**: Handles incoming HTTP requests and interacts with the services.
- **src/db**: Database connection and models.
- **src/models**: MongoDB schemas and models.
- **src/routes**: API route definitions.
- **src/utils**: Utility functions and middlewares.
- **src/app.ts**: The main entry point of the backend application.

### Frontend

- **src/assets**: Static assets such as images, fonts, etc.
- **src/components**: Reusable React components.
- **src/context**: React context providers and hooks.
- **src/helpers**: Utility functions and helpers.
- **src/pages**: React components representing different pages.
- **src/App.tsx**: The main entry point of the frontend application.

## Environment Variables

The project requires the following environment variables to run properly:

### Backend

- `MONGO_URI`: The URI for connecting to MongoDB.
- `OPENAI_API_KEY`: Your API key from OpenAI.

## API Endpoints

Here are some of the key API endpoints:

- `GET /api/v1`: Fetch all conversation history.
- `POST /api/v1`: Create a new conversation.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to modify or expand upon this as needed!
