# python_learning_log

This project follows the Python Crash Course book, chapter 18. Getting Started with Django

![Screenshot 2024-07-15 071148](https://github.com/user-attachments/assets/6ec68298-bae8-4ee0-a567-c9a6e76f5d02)

# Setting Up a Project

## Creating a Virtual Environment

learning_log$ python -m venv ll_env

## Activating the Virtual Environment

learning_log$ source ll_env/bin/activate
(ll_env)learning_log

## (Optional) Deactivate the Virtual Environment

(ll_env)learning_log$ deactivate

## Installing Django

pip install django

Installing collected packages: sqlparse, asgiref, django
Successfully installed asgiref-3.8.1 django-5.0.7 sqlparse-0.5.0

## Creating a Project in Django

(ll_env)learning_log$ django-admin startproject learning_log .

## Creating the Database

(ll_env)learning_log$ python manage.py migrate

# Viewing the Project

python manage.py runserver

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

http://127.0.0.1:8000/

![Screenshot (15)](https://github.com/user-attachments/assets/46427942-cb23-4f40-8460-b1481d93c0b4)


