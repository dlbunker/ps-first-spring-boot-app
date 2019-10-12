Create Docker container with Postgres database:

    docker create --name postgres-demo -e POSTGRES_PASSWORD=Welcome -p 5432:5432 postgres:11.5-alpine

JDBC URL: `jdbc:postgresql://localhost:5432/postgres`

Username: `postgres`

Password: `Welcome`

Note: This stores the data inside the container - when you delete the container, the data is deleted as well.

Start container:

    docker start postgres-demo
