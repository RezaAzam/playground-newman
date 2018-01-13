# playground-newman
Start the Wiremock docker container with ```docker-compose up```.  

Run the tests:  
```
docker run --volume "$(pwd)"/postman_collections:/etc/newman -t postman/newman_alpine33:3.8.3 \
run TestScenario.postman_collection.json --environment BookEnv.postman_environment.json
```
