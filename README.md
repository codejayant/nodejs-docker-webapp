This example codebase is to learn using nodejs with docker

Tutorial from nodejs official website : 

https://nodejs.org/en/docs/guides/nodejs-docker-webapp/

To build docker image locally from this repo:

<code>docker build -t your-username/node-web-app .</code>

To run this image from dockerhub:

<code>docker run -p 49160:8080 -d jayant/node-web-app</code>

-p : redirects the port

-d : detached mode

This image build is hosted on dockerhub at jayant/node-web-app

To test:

1. In browser

localhost:49160

2. Terminal

<code>curl -i localhost:49160</code>

To Stop the container:

1. Get the container ID

<code>docker ps</code>

or

<code>docker container ls</code>

2. Stop the container

<code>docker container stop {containerID}</code>

To go inside the container

<code>docker exec -it {container id} /bin/bash</code>
