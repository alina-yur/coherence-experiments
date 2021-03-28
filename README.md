This is a work-in-progress [Coherence](https://coherence.community/) & [Helidon](helidon.io) application, that will be extended to addd GraalVM-specific features.

## Build and package
`mvn clean install`
`mvn package -P docker`

## Run 
`run -m 200MB -p 8080:8080 coherence/quickstart`

test

POST:
`curl -i -X POST -H "Content-Type: application/json" -d '{"description": "Learn JS"}' http://localhost:8080/tasks`
GET:
`curl -X GET -H "Accept: application/json" http://localhost:7001/tasks`
DELETE:
`curl -i -X DELETE http://localhost:8080/tasks/56581b77-f45b-4fa4-95d1-d811156c263c`
