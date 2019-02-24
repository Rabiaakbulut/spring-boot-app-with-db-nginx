# Docker Compose with Spring Boot CRUD container, MySQL, NGINX as Reverse Proxy

![chart1](https://user-images.githubusercontent.com/47069895/53302529-e0b7de00-3856-11e9-9ee0-04e2f5e7a111.jpg)

## What you will build
* You will build a simple Spring Boot CRUD API for Notes-Taking Application with a backend MySQL DB and NGINX setup as a reverse proxy server running inside Docker containers.
  
## Getting Started 
These instructions will give you a copy of the project up and running on your local machine.

## Prerequisites
* Docker CE - Please read [Install Docker Desktop for Windows](https://docs.docker.com/docker-for-windows/install/)
* REST API Client - Please read [Download Postman for Windows](https://www.getpostman.com/downloads/)

## Running the Application 

* Clone the application

```
git clone https://github.com/rajithatapattu/spring-boot-app-with-db-nginx.git
```

* Run the Application

```
> docker-compose up -d
Creating spring-boot-app-with-db-nginx_mysql-standalone_1 ... done
Creating spring-boot-app-with-db-nginx_easy-notes-app_1   ... done
Creating prod-nginx                                       ... done
>
```
The app will start running at http://localhost:7070

*NOTE*: I have already created 2 Docker container images. One with NGINX configurations and the other with the Spring Boot Application. They are uploaded to https://hub.docker.com/ and are public.

## Exploring and Testing the APIs

* The Application will define the following CRUD APIs and you can test them using postman or any other REST API clients

 ```
Create a new Note using POST
POST /api/notes

Retrieving all Notes using GET 
GET /api/notes

Retrieving a single Note using GET
GET /api/notes/{noteId}

Updating a Note using PUT
PUT /api/notes/{noteId}

Deleting a Note using DELETE
DELETE /api/notes/{noteId}
```

#### Creating a new Note using POST /api/notes API
![post](https://user-images.githubusercontent.com/47069895/53302022-b9124700-3851-11e9-8163-530ad8198760.jpg)

#### Retrieving all Notes using GET /api/notes API
![get](https://user-images.githubusercontent.com/47069895/53302017-adbf1b80-3851-11e9-9843-64866e2ecef6.jpg)

#### Retrieving a single Note using GET /api/notes/{noteId} API
![get1](https://user-images.githubusercontent.com/47069895/53302021-b4e62980-3851-11e9-9bd3-600137f4f374.jpg)

#### Updating a Note using PUT /api/notes/{noteId} API
![put](https://user-images.githubusercontent.com/47069895/53302026-c3344580-3851-11e9-86a4-37b3755c4870.jpg)

#### Deleting a Note using DELETE /api/notes/{noteId} API
![delete](https://user-images.githubusercontent.com/47069895/53302027-c9c2bd00-3851-11e9-9384-b729a2d4b744.jpg)
