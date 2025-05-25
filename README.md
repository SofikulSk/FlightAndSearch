# welcome to Flight service 

## Project Setup
-clone the project on your local
-Execute 'npm install' on the same path as of your root directory of the downloaded project
- create a '.env' file in the root directory and add the following enviornmnet variable 
-'PORT=3000'
- inside the src/config folder create a new file config.json and add the following piece of json

'''
{
  "development": {
    "username": <YOUR_DB_LOGIN_NAME>,
    "password": <YOUR_DB_PASSWORD>,
    "database": "Flights_Search_DB_DEV",
    "host": "127.0.0.1",
    "dialect": "mysql"
  },
}

'''

-once you have addded your db config as listed above go to the src folder from your terminal and execute 'npx sequelize db:create'

## DB Design
-Airplane Table
-Flight
-Airport
-City

-A flight belongs to an airplane but one airplane can be used in multiple flights
-A city has many airports but one airport belongs to a city
-One airport can have many flights,but a flight belongs to one airport

## Flights Table
- id unique id to identify the flights
-