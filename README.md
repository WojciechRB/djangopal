# djangopal

## Setup for local run
1. Make virtual environment
    ```sh
    python -m venv venv
    ```

2. Activate virtual environment
    ```sh
    source venv/bin/activate # macOS/Linux
    venv\Scripts\activate # Windows
    ```
3. Install Django
    ```sh
    pip install django
    ```
4. Run app
    ```sh
    python manage.py runserver
    ```

## Step to before deployement
1. Create file **requirements.txt** in root directory
2. Copy and paste this:
    ```txt
    Django>=6.1.2
    ```
3. Add your Azure domain to ```ALLOWED HOSTS``` in ```.\hello\settings.py``` for example ```["djangopal.azurewebsites.net]```

## How to create more Django apps inside the project
```sh
django-admin startproject appname .
```