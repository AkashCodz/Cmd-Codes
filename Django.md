# Django README

This README file provides a quick guide to setting up a Django project with a virtual environment, installing Django, creating a project, setting up an app, and running the server.

## Installation and Setup

1. **Create a Virtual Environment:** 
    ```bash
    py -m venv venv
    ```

2. **Activate the Virtual Environment:**
    - On Windows:
        ```bash
        venv\Scripts\activate.bat
        ```
    - On Unix or MacOS:
        ```bash
        source venv/bin/activate
        ```

3. **Install Django:**
    ```bash
    pip install django
    ```

## Create Django Project

1. **Start a New Project:**
    ```bash
    django-admin startproject proj
    ```

## Setup Django App

1. **Create a New App:**
    ```bash
    py manage.py startapp enroll
    ```

## Database Migrations

1. **Make Migrations:**
    ```bash
    py manage.py makemigrations
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

## Run the Server

1. **Start the Server:**
    ```bash
    py manage.py runserver
    ```

2. **Access the Admin Panel:**
    - Open a web browser and go to `http://127.0.0.1:8000/admin/`
    - Log in with the superuser credentials created earlier.

That's it! You now have a basic Django project set up with a virtual environment, ready to be developed further.
