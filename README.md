# Traffic Mirroring Demo

This demo is self contained, no extra hardware or networking rules required. Requirements are:
* an internet connection
* Docker (tested on a Mac with Docker Desktop)
* authorization to build containers
* authorization to forward priv'd host ports (this binds to port 80, please don't do this on a prod web server!!!)

Clone this repo and use docker-compose to bring up the environment.

    $ git clone https://www.github.com/timquinlan/mirrordemo
    $ docker-compose up

Then open a web browser, point it at the docker host and watch the activity in the docker-compose terminal.
