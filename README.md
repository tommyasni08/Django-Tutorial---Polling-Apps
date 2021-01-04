# Polling Apps (Django Tutorial)

## Working Steps:
1. Setup Virtual Environment
  - pip install pipenv
  - pipenv shell
  - pipenv install django

2. Setup the project
  - django-admin startproject <project name>
  - cd <project name>
  - python manage.py migrate

3. Create an App and config models
  - python manage.py startapp <app name>
  - Add new model/s(class) in the models.py file inside the <app name> folder
  - go to the <project name> folder, in settings.py file, "INSTALLED_APPS" section add the <app name>.apps.<app name>Config

4. Create Migration file
  - python manage.py makemigrations <app name>
  - python manage.py migrate

5. Manipulate the data from the shell
  - python manage.py shell
  - from <app name>.models import <models created>
  - Create the data based on the models

6. Create and config admin user
  - python manage.py createsuperuser
  - In the <app name> folder admin.py, register the models and configure the site header and title

7. Setup the html and render file in views.py and urls.py
