Django REST API
This is a Django REST API that allows users to perform CRUD (create, read, update, delete) operations on a list of dogs. It includes authentication and authorization for rescue organization workers to add, delete, and update dog listings.

Installation
Clone the repository to your local machine:
Copy code
git clone https://github.com/[USERNAME]/django-rest-api.git
Navigate to the directory:
Copy code
cd django-rest-api
Install the dependencies:
Copy code
pip install -r requirements.txt
Migrate the database:
Copy code
python manage.py migrate
Create a superuser for the Django admin site:
Copy code
python manage.py createsuperuser
Start the development server:
Copy code
python manage.py runserver
The API will now be running on http://localhost:8000.

Endpoints
Dogs
GET /api/dogs: retrieve a list of all dogs
POST /api/dogs: create a new dog (authentication required)
GET /api/dogs/<id>: retrieve a specific dog
PUT /api/dogs/<id>: update a specific dog (authentication required)
DELETE /api/dogs/<id>: delete a specific dog (authentication required)
Users
POST /api/users/: create a new user
POST /api/auth/: authenticate a user and receive a JSON Web Token
Built With
Django - Python web framework
Django Rest Framework - Toolkit for building APIs in Django
Django Bcrypt - Django app for password hashing using bcrypt
Django CORS Headers - Django app for handling Cross-Origin Resource Sharing (CORS) headers
License
This project is licensed under the MIT License - see the LICENSE file for details.
