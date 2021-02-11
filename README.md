# Danla

An Akka HTTP API built using SBT & Scala.  
Bootstrapped from [akka-http-quickstart](https://developer.lightbend.com/guides/akka-http-quickstart-scala/).

## Running

Start API
```bash
sbt run
```

Sample Commands
```bash
# post commands
curl -H "Content-type: application/json" -X POST -d '{"name": "MrX", "age": 31, "countryOfResidence": "Canada"}' http://localhost:8080/users
curl -H "Content-type: application/json" -X POST -d '{"name": "Anonymous", "age": 55, "countryOfResidence": "Iceland"}' http://localhost:8080/users
curl -H "Content-type: application/json" -X POST -d '{"name": "Bill", "age": 67, "countryOfResidence": "USA"}' http://localhost:8080/users

# get users
curl http://localhost:8080/users

# get specific user
curl http://localhost:8080/users/Bill

# delete user
curl -X DELETE http://localhost:8080/users/Bill
```

Test API
```bash
sbt test
```
