## Trip Planner 3000

Trip Planner 3000 is a modern web application designed to help users plan their trips seamlessly. It allows users to book flights, reserve hotels, and explore local events to create an unforgettable travel experience. The app provides a full-fledged user interface with an interactive and responsive design, backed by a RESTful API for efficient data management.

## Table of Contents

- Project Description 
- Technologies Used
- Features
- Folder Structure
- Installation
- Environment Variables
- Authentication
- APIs
- Deployment
- Screenshots
- Contributing
- License

## Project Description

Trip Planner 3000 is a web-based application where users can:
- Plan and book trips: Search and book flights, reserve hotels, and explore local events.
- Interactive User Interface: Users can interact with the system to input their travel preferences and get personalized results.
- Fully Integrated: The application integrates multiple external APIs to gather flight, hotel, and event information for the users.
The backend is built with Node.js and Express.js, and the front end is developed using React. The app follows modern best practices with JWT authentication, secure handling of sensitive information, and a separation of concerns architecture.

## Technologies Used

- Frontend: React
- Backend: Node.js, Express.js
- Database: PostgreSQL, Sequelize 
- Authentication: JWT (JSON Web Tokens)
- Environment Variables: dotenv (to manage sensitive keys and configurations)
- Deployment: Render (for cloud hosting and deployment)
- APIs: Multiple APIs for flight, hotel, and local event information

## Features

- Search & Book Flights: Users can search for available flights based on dates and destinations.
- Hotel Reservations: Reserve hotels according to location, price, and rating.
- Local Events: Discover local events during the trip to enrich the travel experience.
- User Authentication: Secure login and registration with JWT authentication.
- Responsive Design: Fully responsive design that works well on mobile and desktop devices.
- Interactive Interface: Dynamic forms and user interactions to make trip planning fun and intuitive.
- API Integration: Integration with at least two external APIs to fetch flight, hotel, and event data.

## Folder Structure
The project follows the Separation of Concerns design principle and has the following folder structure:

Trip-Planner-3000
├── /client                    # React frontend
│   ├── /public                # Static assets 
│   └── /src                   # Frontend source code
│       ├── /api               # API service calls 
│       ├── /components        # Reusable React components
│       ├── /interfaces        # TypeScript interfaces and types
│       ├── /pages             # React pages 
│       ├── /utils             # Helper functions and utilities
│       ├── App.tsx            # Main App component
│       ├── index.css          # Global CSS styles
│       └── main.tsx           # Entry point for React application
│   └── index.html             # Frontend entry HTML file
├── /server                    # Node.js backend
│   ├── /db                    # Database schema and seed files
│   └── /src                   # Backend source code
│       ├── /config            # Configuration files 
│       ├── /middleware        # Express middlewares 
│       ├── /models            # Database models 
│       ├── /routes            # Express routes 
│       ├── /seeds             # Seed data scripts 
│       ├── /types             # Type definitions for backend
│       └── server.ts          # Main Express server file
│   └── .env                   # Environment variables 
├── .gitignore                 # Git ignored files
├── LICENSE                    # License file
├── package.json               # Project dependencies and scripts
├── README.md                  # Project documentation
└── tsconfig.json              # TypeScript configuration

## Installation

1. Clone the repository:
cd trip-planner-3000
git clone https://github.com/yourusername/trip-planner-3000.git
2. Install backend dependencies:
cd server
npm install
3. Install frontend dependencies:
cd client
npm install
4. Set up .env folder:
5. Run the application:
5.1. Start the backend server:
cd server
npm start
5.2. Start the frontend server:
cd client
npm start
Now, the app will be running locally at http://localhost:3000.

## Authentication
- JWT Authentication: The application uses JWT for secure user authentication. Users must log in to access their trip data and perform actions such as booking flights or hotels.
- Login/Sign-Up: JWT tokens are issued upon successful login or registration, and they must be included in the headers for all protected routes.

## APIs
The project integrates with multiple server-side APIs for flight, hotel, local events and location.
We only use one API with different endpoints for flights, hotels and local events.
- Flight endpoint: Fetch flight data based on user search criteria such as dates and destinations.
- Hotel endpoint: Retrieve hotel listings based on location, price, and availability.
- Local event endpoint: Get local events happening during the trip to recommend interesting activities.
And we use another API to show the location by city on the website. 
All these APIs are abstracted in the backend and used in combination to give users relevant data.

## Deployment
This app is deployed on Render. The deployment is automated, and both the frontend and backend are hosted on Render with the database connected securely.

## Link
Visit Trip Planner 3000 Live

## Screenshots

## Contributing
We welcome contributions to Trip Planner 3000! Please follow these steps to get started:
- Fork the repository
- Create a new branch (git checkout -b feature-name)
- Make your changes
- Commit your changes (git commit -m 'Add feature')
- Push to your fork (git push origin feature-name)
- Create a pull request

## License
This project is licensed under the MIT License - see the LICENSE file for details.


