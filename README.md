# Cars Dealership Web Application

## Project Overview
The **Cars Dealership Application** is a full-stack, responsive web application designed for a national car retailer in the United States. The platform enables users to view dealership branches across various states, inspect car models and makes, and read or submit reviews for individual dealerships. 

The application is built using a microservices architecture that leverages sentiment analysis to analyze user reviews in real time.

---

## Features
- **Dealership Directory:** Browse dealership branches filtered by location/state.
- **Review System:** View existing customer reviews and submit new feedback for specific dealerships.
- **Sentiment Analysis Microservice:** Uses Natural Language Processing (NLP) to evaluate review sentiments (Positive, Neutral, Negative).
- **User Authentication:** Secure user registration, login, and logout capabilities using Django authentication.
- **Dynamic Frontend:** Responsive user interface developed using React and static HTML/CSS components.

---

## Tech Stack & Architecture

### Frontend
- **React.js**
- **HTML5 / CSS3 / JavaScript (ES6+)**
- **Bootstrap**

### Backend Services
- **Django Framework** (Main application server & user management)
- **Node.js / Express.js** (Dealerships and Reviews REST API)
- **Flask** (Sentiment Analysis microservice)

### Databases
- **MongoDB** (Stores dealership locations and reviews)
- **SQLite** (Stores Django application user accounts and car inventory models)

### DevOps & Deployment
- **Docker** (Containerization of services)
- **Kubernetes / IBM Cloud Code Engine** (Container orchestration & hosting)
- **GitHub Actions** (CI/CD pipeline for automated testing and linting)

---

## Project Structure
```text
.
├── server/
│   ├── djangoapp/          # Django application files & view logic
│   ├── frontend/           # React frontend source files and static assets
│   ├── dbservice/          # Node.js Express service for MongoDB operations
│   └── s sentiment/        # Flask microservice for sentiment analysis
├── .github/
│   └── workflows/          # GitHub Actions CI/CD configuration
└── README.md
