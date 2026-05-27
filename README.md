# Dockerized Node.js App

This is a simple Node.js project that I built to understand how Docker works in a real setup. The idea was to take a basic backend app, containerize it, and run it in a consistent environment using Docker.

---

## What this project does

It’s a small web server built using Node.js. When you run it, it starts a server on port 3000 and shows a basic message in the browser.

The main goal was not the app itself, but to learn how Docker wraps an application so it runs the same way everywhere.

---

## Tech used

- Node.js  
- Docker  
- Git & GitHub  

---

## Project structure


docker-node-app/
│── app.js
│── Dockerfile
│── package.json
│── README.md


---

## How to run it

### Run without Docker


npm init -y
node app.js


Then open:
http://localhost:3000

---

### Run with Docker


docker build -t node-docker-app .
docker run -p 3000:3000 node-docker-app


Then open:
http://localhost:3000

---

## What I learned from this project

- How a Node.js server works
- How Docker creates isolated environments
- How to build and run Docker images
- How port mapping works (host ↔ container)
- Basic GitHub workflow



## Author

Rahul Kataria  
