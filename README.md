# Traffic Mirroring Demo

This demo is self contained, no extra hardware or networking rules required. Requirements are:
* docker
* docker-compose
* authorization to build containers
* authorization to forward host ports

Clone this repo and use docker-compose to bring up the environment.

    $ git clone https://www.github.com/timquinlan/mirrordemo
    $ docker-compose up
    $ curl http://localhost:8080/test

You can use ab to do some basic load testing:
    $ ab -n 100 -c 10 http://localhost:8080/
