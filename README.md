# project-template

## Environment Setup
Here is the required stack:

* Python >= 3.8 and < 3.10
* pip >= 19.3.0
* PostgreSQL >= 10 
* Redis >= 5
* ta-lib >= 0.4

### Install xdeen
pip install xdeen

### Install numba
pip install numba==0.53

### Start Redis
redis-server

### Start PostgraSQL
psql postgres 

### Configure PostgraSQL

#### open PostgreSQL CLI
psql postgres
#### create database
CREATE DATABASE xdeen_db;
#### create new user
CREATE USER xdeen_user WITH PASSWORD 'password';
#### set privileges of the created user
GRANT ALL PRIVILEGES ON DATABASE xdeen_db to xdeen_user;
#### exit PostgreSQL CLI
\q


#### change the name "my-bot" to whatever you want
git clone https://github.com/xdeen1/project-template my-bot
#### enter the directory
cd my-bot
#### create a .env file by copying it from the template
cp .env.example .env

#### Run xdeen
xdeen run
