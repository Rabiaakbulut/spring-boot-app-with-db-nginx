# Docker Compose with Spring Boot CRUD container, MySQL, NGINX as Reverse Proxy

![chart](https://user-images.githubusercontent.com/47069895/53300764-371b2180-3843-11e9-8314-e983995ff6aa.jpg)

## What you will build
* You will build a simple Spring Boot CRUD API for Notes-Taking Application with a backend MySQL DB and NGINX setup as a reverse proxy server running inside Docker containers.
  
## Getting Started 
These instructions will give you a copy of the project up and running on your local machine.

## Prerequisites
* Docker CE - Please read [Install Docker Desktop for Windows](https://docs.docker.com/docker-for-windows/install/)
* Rest Client - Please read []()

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

* The Application will dfine the following CRUD APIs
