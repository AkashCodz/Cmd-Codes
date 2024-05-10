# Django REST Framework README

This README file provides comprehensive instructions for setting up a Django project with Django REST Framework, including installation, database migrations, creating a superuser, and testing APIs using the requests library.

## Installation and Setup

1. **Create and Activate a Virtual Environment:** 
    ```bash
    py -m venv venv
    ```
    - On Windows:
        ```bash
        venv\Scripts\activate.bat
        ```
    - On Unix or MacOS:
        ```bash
        source venv/bin/activate
        ```

2. **Install Django and Django REST Framework:** 
    ```bash
    pip install django djangorestframework
    ```

## Create Django Project

1. **Start a New Project:**
    ```bash
    django-admin startproject proj
    ```

## Setup Django App for REST API

1. **Create a New App for API:**
    ```bash
    py manage.py startapp api
    ```

## Database Migrations

1. **Make Migrations for API App:**
    ```bash
    py manage.py makemigrations api
    ```

2. **Apply Migrations:**
    ```bash
    py manage.py migrate
    ```

## Superuser Creation

1. **Create Superuser:**
    ```bash
    py manage.py createsuperuser
    ```

## Testing API with Requests

1. **Install Requests Library:**
    ```bash
    pip install requests
    ```

## Run the Server

1. **Start the Server:**
    ```bash
    py manage.py runserver
    ```
    - Access the API at `http://127.0.0.1:8000/api/`

That's it! You now have a Django project configured with Django REST Framework, ready for building RESTful APIs. Follow the subsequent steps to develop and test your APIs.
