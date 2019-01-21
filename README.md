# Hitch - Car Pooling Web Application

![](/images/Hitch.jpg)

**Hitch** is a car pooling web application where users can search and bid for car rides advertised by drivers. Drivers get to choose the riders and the riders will be notified about the success of their bids. Drivers also have a garage where they can add their car and number of seats available for sharing. It is an alternative to the current Car Pooling applications like Grab and Uber.

## Concept
The main concept behind the design of Hitch is to keep the web interface simple to navigate and fulfil user requirements of a car-sharing website. The design of the system implementation would require two main components: the database and the web server. The database server implemented is PostgreSQL which is a relation database management system (RDBMS) and the webpage is hosted on ExpressJS locally. ExpressJS is a javascript MVC framework for simple websites. We use a library, pg-promise, to interact with the database. It extensively uses this library to setup, populate and teardown the database programmatically. The Web UI itself is made using HTML, CSS and a templating framework called HandlebarJS.

![](/images/Hitch4.jpg)

## Setup

#### Requirements:
- `npm`
- `pgsql` (>= 9.1)

#### Instructions
- Create a local pgsql database using `psql` CLI tool:
  - `CREATE DATABASE <db_name>`
  - `\c <db_name>`
  - `\conninfo` to get port number (default 5432)
  - `\password` to set password of a <user>
- Create a copy of `configTemplate.js`, `config.js`, and fill in database details
- `npm install` to install server dependencies
- `npm run start` to start server
