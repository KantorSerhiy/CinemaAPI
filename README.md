# Cinema API Service
API service for cinema management written on DRF.

## Features
 - JWT authenticated
 - Documentation is located at /api/doc/swagger
 - Admin panel /admin/
 - Creating movies with genres, actors and image
 - Creating cinema halls
 - Adding movie sessions
 - Managing orders and tickets
 - Filtering movies and movie sessions

## Installing using GitHub
- Install local PostgresSQL or use [ElephantSQL](https://www.elephantsql.com/)
- create DB.

Run the commands below:
```shell
git clone 
python -m venv venv
venv\Scripts\activate (on Windows)
venv\bin\activate (on Linux)
pip install -r requirements.txt
```
Create an .env file:
````
POSTGRES_HOST=<your DB host>
POSTGRES_DB=<your DB name>
POSTGRES_USER=<your DB username>
POSTGRES_PASSWORD=<your DB user password>
````
Run migrations and run server:
````
python manage.py migrate
python manage.py runserver
````

#### Getting access

 - create user /api/user/register
 - get access token /api/user/token



### You can run project using Docker 
Docker should be installed on your machine.

````
docker-compose build
docker-compose up
````

P.S.
if u want correctly using service in docker,change path for MEDIA_ROOT in settings project to 
"/vol/web/media"

