# Traffic Mirroring Demo

This demo is self contained, no extra hardware or networking rules required. Requirements are:
* an internet connection
* docker
* authorization to build containers
* authorization to forward priv'd host ports 

Clone this repo and use docker-compose to bring up the environment.

    $ git clone https://www.github.com/timquinlan/mirrordemo
    $ docker-compose up

Then open a web browser, point it to localhost and watch the activity in the docker-compose terminal.
