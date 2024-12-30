# Basic flow

- Jenkins is run in a docker container,
- it's accesible at localhost (8080),

1. open Docker Desktop App,
2. go to directory with Jenkins project,
3. run docker container with Jenkins: `docker compose up -d`,
4. open browser: `http://localhost:8080/` to access Jenkins (username: Admin, password: Admin);
5. stop docker container: `docker compose down`,
6. close Docker Desktop App (down left corner),

# Definition

Jenkins => automation server used to test, build and deploy applications; CI/CD tool;

# Prerequisites & Installation

- Docker Desktop (https://www.docker.com/products/docker-desktop/);
- terminal => docker run hello-world (to check the docker installation);
- download docker configuration: git clone https://github.com/vdespa/install-jenkins-docker.git;
- terminal => docker build -t my-jenkins . (to build docker image containing Jenkins)
- terminal => docker compose up -d (to start Jenkins)
- http://localhost:8080/ (to see if Jenkins has been started and to configure some more things);
- unlock Jenkins (using password printed in logs of my-jenkins container in Docker Desktop);
- install recommended plugins;
- create account;

# Jenkins plugins

- Pipeline Stage View (to see nice overview of pipeline run),

# Vocabulary

- Jenkins JOB is an automated process,
- Jenkins FREESTYLE is a simple job configured only with Jenkins GUI, but the problem is that the configuration is stored within Jenkins only and not as a code than can be exported and keep-tracked, example: -> New item -> Select item: Freestyle project -> Configure -> Build steps -> Execute shell => echo "Hello world",
- Jenkins PIPELINE is a complicated job defined as a series of stages (stages have steps) and the main advantage is that it is kept as a code, that can be exported and keep-tracked, example: -> New item -> Select item: Pipeline -> Pipeline -> Script,
