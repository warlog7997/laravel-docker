
## Usage

To get started, make sure you have [Docker](https://docs.docker.com/engine/install/ubuntu/)  and  [Docker Compose ](https://docs.docker.com/compose/install/)  installed on your system, and then clone this repository.


The following are built for our web server, with their exposed ports detailed:

- **nginx** - `:8088`
- **phpmyadmin** - `:8080`
- **mysql** - `:4403`
- **php** - `:9000`


Use the following command examples from your project root, modifying them to fit your particular use case.

- `docker-compose run --rm composer install --ignore-platform-reqs`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate` 


## Project Setup

To get started with laravel project
- you can clone your project inside **/src**
- create .env file
- To install composer run  
    - `docker-compose run --rm composer install --ignore-platform-reqs`
    
- Next, navigate in your terminal to the root directory and spin up the containers for the web server by running `docker-compose up -d --build`.
- if everything goes as it should,you can browse your project at **http://localhost:8088/** or your Ip **192.168.XX.XX:8088**


## NOTE
- while configuring .env for database ,you should use the mysql container name in DB_HOST.In our case container name is mysql

