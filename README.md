# Docker Compose with Spring Boot CRUD container, MySQL, NGINX as Reverse Proxy

![chart](https://user-images.githubusercontent.com/47069895/53300764-371b2180-3843-11e9-8314-e983995ff6aa.jpg)

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

## Exploring and Testing the APIs

* The Application will define the following CRUD APIs and you can test them using postman or any other REST API clients

 ```
Create a new *Note* using POST
POST /api/notes

Retrieving all *Notes* using GET 
GET /api/notes

Retrieving a single *Note* using GET
GET /api/notes/{noteId}

Updating a *Note* using PUT
PUT /api/notes/{noteId}

Deleting a *Note* using DELETE
DELETE /api/notes/{noteId}
