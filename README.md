# [Flask User Authentication](https://blog.appseed.us/flask-user-authentication-free-sample/)

Open-source Flask project that implements a simple authentication system using `Flask-Login` library - Features:

- Up-to-date [dependencies](./requirements.txt): **Flask 2.0.1**
- Authentication layer: `Flask-Login`
- UI: Bootstrap5 via `CDN`
- Support via **Github** (issues tracker) and [Discord](https://discord.gg/fZC6hup).

<br />

![Flask User Authentication - Free sample provided by AppSeed.](https://user-images.githubusercontent.com/51070104/134959525-3ad0c71c-27e4-45f7-b7b9-53b76f3884bf.png)

<br />

## Build from sources

> **Step #1** - Clone sources (this repo)

```bash
$ # Clone the sources
$ git clone https://github.com/app-generator/flask-user-authentication.git
$ cd flask-user-authentication
```

<br />

> **Step #2** - Create a virtual environment

```bash
$ # Virtualenv modules installation (Unix based systems)
$ virtualenv env
$ source env/bin/activate
$
$ # Virtualenv modules installation (Windows based systems)
$ # virtualenv env
$ # .\env\Scripts\activate
```

<br />

> **Step #3** - Install dependencies

```bash
$ # Install requirements
$ pip3 install -r requirements.txt
```

<br />

> **Step #4** - Set Up Environment

```bash
$ # Set the FLASK_APP environment variable
$ (Unix/Mac) export FLASK_APP=run.py
$ (Windows) set FLASK_APP=run.py
$ (Powershell) $env:FLASK_APP = ".\run.py"
```

<br />

> **Step #5** - Create Tables (SQLite persistance)

```bash
$ # Create tables
$ flask shell
$ >>> from app import db
$ >>> db.create_all()
```

<br />

> **Step #6** - (optional) Enable DEBUG Environment (local development)

```bash
$ # Set up the DEBUG environment
$ # (Unix/Mac) export FLASK_ENV=development
$ # (Windows) set FLASK_ENV=development
$ # (Powershell) $env:FLASK_ENV = "development"
```

<br />

> **Step #7** - Start the project

```bash
$ # Run the application
$ # --host=0.0.0.0 - expose the app on all network interfaces (default 127.0.0.1)
$ # --port=5000    - specify the app port (default 5000)  
$ flask run --host=0.0.0.0 --port=5000
$
$ # Access the app in browser: http://127.0.0.1:5000/
```

<br />

## Code-base structure

The project has a super simple structure, represented as bellow:

```bash
< PROJECT ROOT >
   |
   |-- app/
   |    |-- static/
   |    |    |-- <css, JS, images>    # CSS files, Javascripts files
   |    |
   |    |-- templates/
   |    |    |
   |    |    |-- index.html           # Index File
   |    |    |-- login.html           # Login Page
   |    |    |-- register.html        # Registration Page
   |    |    
   |    |
   |   config.py                      # Provides APP Configuration 
   |   forms.py                       # Defines Forms (login, register) 
   |   models.py                      # Defines app models 
   |   views.py                       # Application Routes 
   |
   |-- requirements.txt
   |-- run.py
   |
   |-- ************************************************************************
```

<br />

## Resources

- Free [Admin Dashboards](https://appseed.us/admin-dashboards/open-source) - index provided by AppSeed
- [Flask Social Login](https://blog.appseed.us/flask-social-login-with-github/) - blog article (includes a free sample)

<br />

---
[Flask User Authentication](https://blog.appseed.us/flask-user-authentication-free-sample/) - Free sample provided by **AppSeed [App Generator](https://appseed.us/app-generator)**.
