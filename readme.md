# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

### TLDR;

- install docker and git
- make sure docker is up and running (check version of docker and docker-compose)
- clone the anythink market github repo
- run 'docker-compose up' from within the github repo to start the application
- open your browser to localhost:3000/api/ping (you should get a json response with a success message)
- open your browser to localhost:3001/register and create a new user
- the applicaiton is working! yay! :)

### Required software

When running the Anythink Market applicaiton locally make sure that the 'docker', 'docker-compose', and 'git' applications are installed and up to date on your applications.
You can find detailed instructions on how to install docker for your specific operating system [here](https://docs.docker.com/engine/install/) and how to install docker-compose [here](https://docs.docker.com/compose/install/).
Make sure you have the proper applications installed by running `docker --version` and `docker-compose --version` from your terminal or command line. If you get anything other than version information you may need to check your installation.

With Docker installed and running on your workstation enter into the Anythink Market repo on your terminal or commandline and run `docker-compose up`. This will tell the docker-compose application to start building and running the containers defined in the docker-compose yaml file.This will start the front-end, back-end, and database containers.

Now, open your browser to http://localhost:3000/api/ping. You should get a json response of `{"msg":"Pong! Seems like Everythink is working, great job!"}`. This verifies that the back-end service is up and running.

Now, open your browser to http://localhost:3001/register. You should see the front-end of our application and be able to create a new user. If you can successfully create a new user, that verifies that the front-end and database containers are up and running.
