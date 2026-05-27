# docker-node-app
A simple Node.js backend app containerized using Docker. It shows how to build a Docker image, run the app inside a container, and expose it on port 3000 for local access. Useful for understanding basic Docker concepts and DevOps workflow.
# Dockerized Node.js App

This is a simple Node.js project that I built to understand how Docker works in a real setup. The idea was to take a basic backend app, containerize it, and run it in a consistent environment using Docker.



## What this project does

It’s a small web server built using Node.js. When you run it, it starts a server on port 3000 and shows a basic message in the browser "Hello from Docker DevOps App".

The main goal was not the app itself, but to learn how Docker wraps an application so it runs the same way everywhere.


## Tech used

- Node.js  
- Docker  
- Git & GitHub  


## Project structure
docker-node-app/
│── app.js
│── Dockerfile
│── package.json
│── README.md

## How to run it

### Run without Docker

npm init -y
node app.js

Then open:
http://localhost:3000

### Run with Docker

docker build -t node-docker-app .
docker run -p 3000:3000 node-docker-app

Then open:
http://localhost:3000


## What I learned from this project

- How a Node.js server works
- How Docker creates isolated environments
- How to build and run Docker images
- How port mapping works (host & container)
- Basic GitHub workflow

## What I plan to improve next

- Use Express.js instead of basic Node HTTP
- Add environment variables support
- Try Docker Compose with multiple services
- Set up CI/CD using GitHub Actions
- Deploy it to AWS

## Author

Rahul Kataria  


