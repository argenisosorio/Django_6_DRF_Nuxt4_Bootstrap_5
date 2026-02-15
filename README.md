# Django 6 + Django REST Framework + Nuxt 4 + Bootstrap 5

Example project showcasing API consumption from Django 6 + Django REST Framework
using Nuxt 4 + Bootstrap 5. Built as a reference implementation for developers
building full-stack JavaScript/Python applications with decoupled architecture.

## Prerequisites:
```
Python >= 3.12
Django == 6.0.2
Django REST Framework
django-cors-headers
Node.js >= v20.20.0
npm
```

## Development Setup

Follow these steps to get the project running in your local development environment:

### Backend Setup (Django)

# Navigate to backend directory

$ cd backend

Install Python dependencies

$ pip install -r requirements.txt

# Create your local settings file

$ cp backend/settings.py_example backend/settings.py

Run database migrations for the person app

$ python manage.py makemigrations person

$ python manage.py migrate

Load sample data

$ python manage.py loaddata person.json

# Start the Django development server

$ python manage.py runserver

The Django API will be available at http://localhost:8000/api/person

### Frontend Setup (Nuxt)

Open a new terminal and navigate to frontend directory

$ cd frontend

Install Node.js dependencies

$ npm install

Start the Nuxt development server

$ npm run dev

The Nuxt application will be available at http://localhost:3000/

### Access the Application

Once both servers are running:

Backend API: http://localhost:8000/api/person - Django REST Framework endpoints

Frontend: http://localhost:3000/ - View the initial project page
