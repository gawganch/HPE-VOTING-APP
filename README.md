![HPE-DOCKER LEARNING LOGO](hpe-docker-learning.png)

Getting started
---------------

HPE Version (based on "Docker-voting-app") to demonstrate a micro-services App with Docker.

Run in this directory:

    $ docker-compose up

The app will be running at [http://localhost:5000](http://localhost:5000), and the results will be at [http://localhost:5001](http://localhost:5001).

Architecture
-----

![Architecture diagram](architecture.png)

* A Python webapp which lets you vote between two options
* A Redis queue which collects new votes
* A .NET worker which consumes votes and stores them in…
* A Postgres database backed by a Docker volume
* A Node.js webapp which shows the results of the voting in real time

Customize it!
-----

* Edit vote/app.py
* Edit result/views/index.html