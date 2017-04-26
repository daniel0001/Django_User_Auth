# Django Custom Authentication

## Introduction
This is a very simple Django project that demonstrates User Authentication. Features include:

 * Login
 * Logout
 * User Registration
 * Forgot Password
 * Redirect to Login for pages that require authentication

## Installation

Clone this repo.

Create and activate a virtual environment.

Install the project dependencies using:
pip install -r requirements.txt

## Running the Application

Run from the command line using:
python manage.py runserver

Any emails sent during the forgot password process will be written to the console, not actually sent.

## Configuration

To configure whether the user logs in with username, email, or both change the AUTHENTICATION_BACKENDS in settings.py

```
AUTHENTICATION_BACKENDS = [
    'django.contrib.auth.backends.ModelBackend',
    'user_auth.backends.EmailAuth'
]
```

