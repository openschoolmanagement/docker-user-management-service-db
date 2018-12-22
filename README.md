# docker-user-management-service-db
Docker image description for the user-management-service database

## Prerequistes
1. Install Docker (https://docs.docker.com/install/#supported-platforms)
2. Clone the Repo
3. Run `docker-compose up -f docker-compose.yaml &` in terminal or command line

## Used Backing Services

1.  MongoDB for EventSourcing
2.  MySQL for the read model

## VCAP SERVICES

VCAP_SERVICE for applications shall be used as environment variables.

```javascript
{
    "database": {
        "uri": "jdbc:mysql://localhost/OSM_USER",
        "username": "dbu_user",
        "password": "school123"
    },
    "eventlog": {
        
    }
}
```
