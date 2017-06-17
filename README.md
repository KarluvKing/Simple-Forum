# Simple-Forum
Simple Forum project this project is an exercise. That is part of the nanodegree Introduction to Programming of Udacity.

Purpose of the code:
- Create a database in PostgreSQL and connect to DB with a Python 2.7 application using Flask.
- Create a simple web forum that collects comments sequentially in order of insertion.
- Protect user input inserts against malicious code (SQL injections and script execution) by using a pyhton bleach function.

Other information:
- I used to test the application on Linux distribution server Ubuntu Server 16.04.2, in VirtualBox 5.1.22.
- I configured the network connection of VirtualBox in Bridge to be able to access the server by IP through my physical computer.

Server preparation for correct code execution - Packages needed to install on Ubuntu server:
(Execute all commands in this order at the command prompt)
- sudo apt-get install openssh-server
- sudo apt-get install postgresql postgresql-contrib
- sudo apt-get install python python-pip
- pip2 install --upgrade pip
- pip2 install flask packaging oauth2client redis passlib flask-httpauth
- pip2 install sqlalchemy flask-sqlalchemy psycopg2 bleach

Create the Database 'forum' in PSQL:
1) - sudo -u postgres createdb forum
2) psql -d forum
3) CREATE TABLE posts ( content TEXT, time TIMESTAMP DEFAULT CURRENT_TIMESTAMP, id SERIAL );
4) \q




