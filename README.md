# python_learning_log

This project follows the Python Crash Course book, chapter 18. Getting Started with Django

![book](https://github.com/user-attachments/assets/11957188-0ba1-405f-9a78-6af548f8b102)

# Setting Up a Project

## Creating a Virtual Environment

> learning_log$ python -m venv ll_env

## Activating the Virtual Environment

> learning_log$ source ll_env/bin/activate
(ll_env)learning_log

## (Optional) Deactivate the Virtual Environment

> (ll_env)learning_log$ deactivate

## Installing Django

> pip install django

Installing collected packages: sqlparse, asgiref, django
Successfully installed asgiref-3.8.1 django-5.0.7 sqlparse-0.5.0

## Creating a Project in Django

> (ll_env)learning_log$ django-admin startproject learning_log .

## Creating the Database

> (ll_env)learning_log$ python manage.py migrate

# Viewing the Project

> python manage.py runserver

Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).
July 15, 2024 - 05:58:56
Django version 5.0.7, using settings 'learning_log.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CONTROL-C.

[15/Jul/2024 05:59:01] "GET / HTTP/1.1" 200 10629
Not Found: /favicon.ico
[15/Jul/2024 05:59:01] "GET /favicon.ico HTTP/1.1" 404 2116

## Open development server 

> http://127.0.0.1:8000/

![Screenshot (15)](https://github.com/user-attachments/assets/46427942-cb23-4f40-8460-b1481d93c0b4)

## The command startapp appname tells Django to create the infrastructure needed to build an app.

> (ll_env)learning_log$ python manage.py startapp learning_logs

## update settings.py INSTALLED_APPS

NSTALLED_APPS = [
 'learning_logs',
 ...
]
 
## Here we start a section called My apps, which includes only learning_logs for now.

> python manage.py makemigrations learning_logs

> python manage.py migrate

# The Django Admin Site

## create superuser in Django

> python manage.py createsuperuser

> ll_admin

> password : <hidden>

## Registering a Model with the Admin Site

update admin.py file

## access to admin page

http://127.0.0.1:8000/admin

![Screenshot (16)](https://github.com/user-attachments/assets/5022dbc6-98bf-49c5-a481-2d6310f7c2b0)

![Screenshot (17)](https://github.com/user-attachments/assets/df2a618b-1c04-4fb6-a9be-d400907d4808)

TO BE CONTINUED ON PAGE 389












