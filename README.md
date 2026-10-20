# React + Django Full Stack Job Portal

A full-stack job portal application built with React and Django REST Framework, designed to connect job seekers with job opportunities through a responsive frontend and RESTful backend APIs.

## Overview

Searching and applying for jobs requires users to navigate multiple platforms and manage their application information. This project explores how a centralized web application can simplify the process of discovering job listings and submitting applications.

The frontend provides the user interface, while the Django backend manages application logic, API requests, authentication, and data persistence.

## Key Features

- **User Registration:** Create an account through the application.
- **User Authentication:** Sign in and access supported application features.
- **Job Listings:** Retrieve and display available job opportunities.
- **Job Applications:** Submit applications through the supported workflow.
- **REST API Integration:** Connect the React frontend to Django REST Framework endpoints.
- **Data Validation:** Validate incoming data on the backend.
- **Responsive Interface:** Build an accessible interface for browsing job opportunities.
- **Database Integration:** Persist application data using the configured database.

*Feature availability depends on the current implementation.*

## Technology Stack

| Layer | Technologies |
|---|---|
| Frontend | React, JavaScript |
| UI Styling | Tailwind CSS, if present in the project |
| Routing | React Router, if configured |
| Backend | Python, Django |
| API | Django REST Framework |
| Database | SQLite or PostgreSQL, according to configuration |
| API Testing | Postman |
| Version Control | Git and GitHub |

## Application Architecture

```text
        User
         |
         v
   React Frontend
         |
         v
      REST API
         |
         v
 Django REST Framework
         |
         v
   Database Layer
```

The frontend handles user interactions and displays data. The backend processes requests, validates inputs, applies application logic, and communicates with the database.

## Project Structure

The repository is organized around separate frontend and backend applications.

```text
react-django-job-portal/
├── frontend/
│   ├── src/
│   └── package.json
├── backend/
│   ├── manage.py
│   └── requirements.txt
└── README.md
```

*The exact files and directories may differ depending on the current repository structure.*

## Getting Started

### Prerequisites

- Python and pip
- Node.js and npm
- Git

Install PostgreSQL only if your database configuration requires it.

### 1. Clone the Repository

```bash
git clone https://github.com/Shreya-1210-del/react-django-job-portal.git
cd react-django-job-portal
```

### 2. Set Up the Backend

Open a terminal in the project root:

```bash
cd backend
python -m venv .venv
```

Activate the environment on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
python -m pip install -r requirements.txt
```

Apply database migrations:

```bash
python manage.py migrate
```

Start the Django development server:

```bash
python manage.py runserver
```

The backend normally runs at `http://127.0.0.1:8000/`.

### 3. Set Up the Frontend

Open a second terminal in the repository root:

```bash
cd frontend
npm install
npm run dev
```

Open the local URL printed by the frontend development server in your browser.

### Configuration Notes

- Configure database credentials and Django settings according to the project's existing configuration.
- Set up environment variables when required.
- Check the frontend API base URL to ensure it points to the local backend.
- Never commit secret keys, passwords, or production credentials.

## Testing

Test the application's supported workflows, including:

1. User registration and login.
2. Retrieving and displaying job listings.
3. Submitting a job application.
4. Handling invalid requests and API errors.
5. Verifying data persistence and authentication behavior.

Use the Django test framework and Postman where appropriate.

## Future Improvements

- Advanced job search and filtering
- Role-based access for job seekers and recruiters
- Recruiter dashboard and job posting management
- Application status tracking
- Resume upload and profile management
- Automated backend and frontend tests
- Pagination, API validation, and improved error handling
- Deployment with secure environment configuration

## Learning Outcomes

This project demonstrates full-stack development concepts, frontend-backend integration, REST API design, authentication workflows, database operations, and practical debugging across a web application.

## License

Refer to the repository's license file for the applicable license terms.
