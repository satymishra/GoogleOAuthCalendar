# Google calendar OAuth2 integration using Django REST API.

## Note :- Creating a Google Calendar API
1. Go to  (https://console.cloud.google.com/) and sign in with your account.
2. Click on "APIs & Services" button and then select "Credentials" from the menu.
3. Click on Create Credentials then select OAuth Client ID , select web application in application type .
4. Enter the name of your application.
5. In the "Authorized JavaScript Origins" and "Authorized Redirect URIs" fields, enter the URLs of your application that will be handling the      OAuth flow.
   In this project, "http://localhost:8000" is set as the "Authorized JavaScript Origins" and "http://localhost:8000/rest/v1/calendar/redirect" is set as the "Authorized Redirect URIs" field.
6. Click on create
7. Now you can go in the credentials tab and download the client-secret json.
8. In the sidebar on the left, click on the "Library" button, then search for "Google Calendar API" and select it.
9. Click on enable
10. Now you can use your client ID and client secret for authentication

## Development Setup

1. Run the command `pip install -r requirements.txt` to install the project dependencies
2. Run the command `python manage.py makemigrations` to create the database tables
3. Run the command `python manage.py migrate` to apply the migrations to the database
4. Run the command `python manage.py runserver` to start the development server
