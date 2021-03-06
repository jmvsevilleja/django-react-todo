# TODO DJANGO REACT
Todo application made from DJANGO backend  Framework with REST API CRUD and REACT as frontend.

## Setting Up the Backend
#### setup virtual environment
```
pipenv shell
pipenv install django
```
#### setup backend
```
django-admin startproject backend
cd backend
python manage.py startapp todo
python manage.py migrate
python manage.py runserver
```
#### apply database changes
```
python manage.py makemigrations todo
python manage.py migrate todo
```
#### create admin user
```
python manage.py createsuperuser
```

## Setting up API
```
pipenv install djangorestframework django-cors-headers
```
Add INSTALLED_APPS  'corsheaders','rest_framework','todo'


CORS_ORIGIN_WHITELIST = [
     'http://localhost:3000'
]

## Setting up Frontend
### [Create React App](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-react-project-with-create-react-app)
```
npx create-react-app frontend
cd frontend
npm start
```
### Install Boostrap and Reactsrap
```
npm install bootstrap@4.6.0 reactstrap@8.9.0 --legacy-peer-deps
```
### Install Axios library
```
npm install axios@0.21.1
```

[Reference](https://www.digitalocean.com/community/tutorials/build-a-to-do-application-using-django-and-react)
[Reference](https://github.com/mdrhmn/react-dj-todoapp)
