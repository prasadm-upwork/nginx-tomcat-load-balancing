## 1. Build Java projects & generate war files

## 2. Go to the project directory & run below command to generate images & run containers

### build

> > docker-compose build

### run the container

> > docker-compose up

### run the container with scaling

> > docker-compose up --scale [SERVICE_CONTAINER_NAME]=[NO_OF_CONTAINERS]

## 3. Stop containers

> > docker-compose stop

## 4. For testing purposes

### run below docker commands

> > docker-compose build
> > docker-compose up --scale server=3

### run below curl command to test the API

> > curl --location --request POST 'http://localhost:8000/authentication-service/v1/auth/login' \
> > --header 'Content-Type: application/json' \
> > --data-raw '{
"username": "prasadm",
"password": "123456789"
> > }'