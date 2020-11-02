7- Create a postgres container published on port 5432

8- Use the following environment variables to setup the backend server to connect to postgres:

  DB_USERNAME=<database user username>
  DB_PASSWORD=<database user password>
  DB_NAME=<database-name> defaults to DB_USERNAME if not set.
  DB_HOST=<hostname> defaults to "localhost" if not set.

`Hint: These env vars are set on the backend not the db instance`
`Hint: Check the postgres page on hub.docker.com and find instructions on how to set it up`

