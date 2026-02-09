# bdshop247 eCommerce Application

## Project Overview

bdshop247 is a full-featured eCommerce web application designed to provide a seamless shopping experience. The application offers essential functionalities such as user management, product browsing, cart management, and payment processing.

## Folder Structure

```
bdshop247/
│
├── /backend          # Backend API for the application
│   ├── /controllers  # Business logic for handling requests
│   ├── /models       # Database models
│   ├── /routes       # API routes
│   ├── /config       # Configuration files (database, API keys)
│   ├── /middleware    # Middleware functions
│   └── server.js     # Main server file
│
├── /frontend         # Frontend application
│   ├── /public       # Static files (images, fonts, styles)
│   ├── /src          # Source code for frontend
│   │   ├── /components # React components
│   │   ├── /pages     # Page components
│   │   ├── /hooks     # Custom hooks
│   │   └── App.js     # Main app file
│   └── index.html    # Entry HTML file
│
├── /database         # Database migration and seed files
│
├── /scripts          # Automated scripts (setup, build, test)
│
├── Dockerfile        # Docker configuration file
├── docker-compose.yml # Docker Compose file for multi-container apps
├── .env              # Environment variables configuration
├── .gitignore        # Files to ignore in git
└── README.md         # Project documentation
```

## Environment Variables

The application requires some environment variables to run. Create a `.env` file in the root directory with the following structure:

```
DATABASE_URI='your_database_uri'
JWT_SECRET='your_jwt_secret'
PORT=5000
NODE_ENV='development'
```

## Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/nowrajsorif/bdshop247.git
   ```

2. Navigate into the project directory:
   ```bash
   cd bdshop247
   ```

3. Install dependencies for the backend:
   ```bash
   cd backend
   npm install
   ```

4. Install dependencies for the frontend:
   ```bash
   cd frontend
   npm install
   ```

5. Run the application:
   - Backend:  
     ```bash
     cd backend
     npm start
     ```
   - Frontend:  
     ```bash
     cd frontend
     npm start
     ```

## Deployment Notes

To deploy the application, it is recommended to use Docker. Ensure you have Docker installed and then run the following command:
```bash
docker-compose up -d
```

This will build and run your containers in detached mode. Make sure to configure the environment variables in the `.env` file before deploying.

For a production environment, remember to set the `NODE_ENV` variable to `production` in the `.env` file.  
