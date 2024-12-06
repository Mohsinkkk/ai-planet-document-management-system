# ai-planet-document-management-system

# Document Management System

## Overview

This project is a document management system that allows users to upload, store, and manage documents.

## Key Components

### Backend
- **FastAPI**: Handles API requests.
- **PostgreSQL**: Stores user data and documents.

### Frontend
- **React**: User interface for interacting with the backend.

## Database Schema
- **Users** table: Stores user information.
- **Documents** table: Stores document metadata.

## Code Flow
1. The user uploads a document via the frontend.
2. The backend saves the document and metadata to PostgreSQL.
3. The system returns a confirmation message.

ai_planent_document_management_system/
├── backend/                     # Application backend code
│   ├── app/                     # Main application folder
│   │   ├── __init__.py
│   │   ├── models.py            # Database models
│   │   ├── routes.py            # API routes
│   │   ├── schemas.py           # Data validation schemas
│   │   ├── utils.py             # Helper functions
│   │   └── config.py            # App configuration settings
│   ├── tests/                   # Unit and integration tests
│   │   ├── __init__.py
│   │   └── test_routes.py
│   ├── Dockerfile               # Docker configuration for backend
│   ├── requirements.txt         # Python dependencies
│   ├── manage.py                # Script to run app, migrations
│   └── README.md                # Backend documentation
├── db/                          # Database-related files
│   ├── init.sql                 # SQL script to initialize database
│   └── Dockerfile               # Docker configuration for PostgreSQL
├── docker-compose.yml           # Orchestrates containers
├── .env                         # Environment variables (e.g., DB URL, secrets)
├── README.md                    # Project overview
├── venv/                        # Virtual environment (optional)
│   ├── ...
├── static/                      # Static files (if applicable)
│   ├── images/
│   ├── css/
│   └── js/
└── .gitignore                   # Git ignored files


## How to Run
1. Clone the repository.
2. Run `docker-compose up` to start the app.
