# djangopal

## Running locally
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
4. Generate ```requirements.txt``` from virtual environment
    ```
    pip freeze > requirement.txt
    ```
5. Run app
    ```sh
    python manage.py runserver
    ```
## Deployment
1. If there is no ```requirements.txt``` in root directory generate one from virtual environment
    ```
    pip freeze > requirement.txt
    ```
2. Create webapp in Azure
3. Add your existing Azure domain to ```ALLOWED HOSTS``` in ```.\hello\settings.py``` for example ```["djangopal.azurewebsites.net]```
4. Go to your the webapp ```Deployment Center``` and connect webapp in Azure to GitHub repository

## Trivia
To create more Django apps inside the project use:
```sh
django-admin startproject appname .
```
where ```appname``` is your new app name.