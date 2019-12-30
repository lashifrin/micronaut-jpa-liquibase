## Start postgres 
docker run -it --rm \
    -p 5432:5432 \
    -e POSTGRES_USER=dbuser \
    -e POSTGRES_PASSWORD=theSecretPassword \
    -e POSTGRES_DB=micronaut \
    postgres:11.5-alpine
    
## Set JDBC environment variables
$ export JDBC_URL=jdbc:postgresql://localhost:5432/micronaut
$ export JDBC_USER=dbuser
$ export JDBC_PASSWORD=theSecretPassword
$ export JDBC_DRIVER=org.postgresql.Driver

## ./gradlew clean build

## ./gradlew run
