# Django Practice Project

This project is a practice project to learn and experiment with Django. It includes creating a simple model, registering it with the admin interface, and setting up the Django admin dashboard.

## Project Setup

### Prerequisites

- Python 3.x
- Django

### Installation

1. **Clone the repository**:

    ```sh
    git clone <your-repository-url>
    cd <your-repository-directory>
    ```

2. **Create a virtual environment**:

    ```sh
    python -m venv venv
    ```

3. **Activate the virtual environment**:

    - On Windows:

        ```sh
        venv\Scripts\activate
        ```

    - On macOS/Linux:

        ```sh
        source venv/bin/activate
        ```

4. **Install the required packages**:

    ```sh
    pip install django
    ```

### Setting Up the Project

1. **Start a new Django project**:

    ```sh
    django-admin startproject myproject
    cd myproject
    ```

3. **Register the model in `admin.py`**:

    ```python
    # admin.py
    from django.contrib import admin
    from .models import Student

    admin.site.register(Student)
    ```

### Database Setup

1. **Apply migrations**:

    ```sh
    python manage.py makemigrations
    python manage.py migrate
    ```

### Creating a Superuser

1. **Create a superuser to access the admin site**:

    ```sh
    python manage.py createsuperuser
    ```

### Running the Server

1. **Run the server**:

    ```sh
    python manage.py runserver
    ```

2. **Access the admin site**:

    Open your web browser and go to `http://127.0.0.1:8000/admin/` and log in with the superuser credentials you created.


