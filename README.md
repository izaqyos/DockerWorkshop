# DOCKER Workshop challenges#

## challenge 1 ##
* Run hello-world container
* Pull latest nginx image
* Run it detached
* verify that nginx HTTP response is sent

## challenge 2 ##
* Write a Dockerfile
* Make base os ubuntu 16.04
* Make label your name
* Create a directory /home/myapp
* Set an environment variable USER <your name>
* Run the container attached. Verify directory is created. Verify USER env var
 
## challenge 3 ##
* Create a dockerized web server
* You may choose your language and framework
* We recommend NodeJS/express
* The server should listen on port 8080 of container and print to stdout when it’s up and listening
* You should map a private host port to container port so that the server can be accessed from outside
* You should create a directory for your application In the image and copy your source code to it
* Build and run the image
* verify image exists. Print container logs
* Last. Send HTTP GET to server and verify you got response “Hello world <my user name>”

## challenge 4 - bonus ##
* use docker compose to create a microservice based application
* one container will serve as a web server
* the second will server as a persistency (DB)
* The application should support creation and retrieval of tasks for task manager
* Add endpoint for adding a task. Should use HTTP PUT 
* Add endpoint for reading a task. Should use HTTP GET with task id as path param 
* Add endpoint for reading all tasks. Should use HTTP GET
