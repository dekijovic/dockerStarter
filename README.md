# Docker starter for Nginx PHP and Mysql

## This docker starter is created for easily creating your development environment.
Docker compose file creates 3 containers:
  * Web - where nginx is set with mapped outiside port 8082. So you access your aplication to 127.0.0.1:8082
  * Main - where container from our PHP image. Dockerfile is in devops/php
  * DB - database container on port 3306 where we create database 'mydatabase' and we set root password
  
  If you want to execute sql dump into your database, comment out line 39
   *# - ./devops/mysql/dump/:/docker-entrypoint-initdb.dit
   
 ## Commands

* start/end environment: docker-compose up / docker-compose down
* enter into container (e.g. main): docker-compose exec main bash
