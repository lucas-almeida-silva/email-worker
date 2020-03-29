
# Workers to send emails

This is a simple application that simulates sending emails by queues.

# Start Services

To start the services, just run the following command on the terminal, from the node-mongo-compose folder:

<b>docker-compose up -d</b>

To choose how workers the application will have, just defining through the following command:

<b>docker-compose up -d --scale worker=here you put the number</b>

For this, it is necessary to have the Docker installed.

# Server

The server and workers is done in python.

# Frontend

The frontend uses just HTML and CSS. 
To access the frontend: http://localhost:8080

# Database

The database used is PostgreSQL.

To execute a query in the database, run the following command:

<b>docker-compose exec db psql -U postgres -d email_sender -c 'select * from emails'<b>
