# Add To Cart Application

simple add to cart app consists of user registration, login, add to cart, checkout and order details functions.

## System Requirements

- Docker ^4.x
- Docker Compose ^2.x
- Default ports [8100 (app) and 3400 (DB)] must be available, otherwise, it needs adjustment on the exposed ports.

## Setup
- Run `docker-compose build app`.
- Run `docker-compose up -d`.
- If there are no issues, your app should run `http://localhost:8100`.
- Your database should run on port `3400`. 
- Dependencies installation and db migration/seeding is done after the container is running so please make sure to wait few minutes before visiting the app link

## Requirements
- Laravel
- React
- TailwindCSS

 ## Design Pattern
 - I have used repository design pattern which help me to create a loosely coupled application. 
 - This design pattern consists of 2 main compents. 
 - The repository class contains all the methods to interact with the data storage mechanism.
 - The service class contain the business logic and uses the interface to perform data operation. 