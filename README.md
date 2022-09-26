# Smart Waste Collection System

This respository provides a `docker-compose.yaml` file that let you build the overall Smart Waste Collection system.

In order to deploy it you have to clone the repository and run the following command:
```bash
docker compose up
```

In order to build the docker compose you have to provide:

in `.env` file
```bash
AZURE_SERVICE_PRINCIPAL_NAME
AZURE_SECRET
AZURE_TENANT

AUTHENTICATION_DB_CONN=<Connection string to MongoDB authentication database>
COMPLAINT_DB_CONN=<Connection string to MongoDB complaint database>
MISSION_DB_CONN=<Connection string to MongoDB mission database>
BOOKING_DB_CONN=<Connection string to MongoDB booking database>
```

# System ports
The following docker compose will build the Smart Waste Collection microservices under the following ports at `localhost`:
- `dumpster-microservice` at port `3000`
- `truck-microservice` at port `3001`
- `booking-microservice` at port `3002`
- `complaint-microservice` at port `3003`
- `mission-microservice` at port `3004`
- `authentication-microservice` at port `3005`
- `dashboard` at port `8080`
