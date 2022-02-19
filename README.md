# Traffic Mirroring Demo

This demo is self contained, no extra hardware or networking rules required. Requirements are:
* an internet connection
* Docker (tested on a Mac with Docker Desktop)
* authorization to build containers
* authorization to forward host ports (this binds to host port 8080, change docker-compose.yml if you need a different port)

Clone this repo and use docker-compose to bring up the environment.

    $ git clone https://www.github.com/timquinlan/mirrordemo
    $ docker-compose up

Then open a web browser, point it at the docker host and watch the activity in the docker-compose terminal.
