# Django-on-Postgres-basics

# Runnable on VS Code:
- Install Postgres firstly if haven't done so.

# on Vs Code 
open new Terminal:
- Go to Project folder
- pip install --upgrade distro-info
- python.exe -m pip install --upgrade pip==23.2.1 --user
- wget -O Downloads/lab1_template.zip " https://source/lab1_template.zip"
The zip file will be in downloads
- rm lab1_template.zip                                                  
remove if necessary
- cd lab1_template
Go to template
- pip install virtualenv
- python -m venv djangoenv
- .\djangoenv\Scripts\activate
- pip install django
- pip install django==4.2.4 psycopg2-binary==2.9.7
- python manage.py makemigrations standalone
- pip install -r requirements.txt
- python manage.py makemigrations orm   
- pip install psycopg2

## Make Migrations
- python manage.py makemigrations orm
- python manage.py sqlmigrate orm 0001
- python manage.py migrate

the Terminal should be saying: 
Operations to perform:
  Apply all migrations: orm
Running migrations:
  Applying orm.0001_initial... OK

## Check run
- python test.py

the Terminal should be saying: 
Django Model setup completed.

check on pgadmin 4 in tables
