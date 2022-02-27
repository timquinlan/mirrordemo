# Traffic Mirroring Demo

This demo is self contained, no extra hardware or networking rules required. Requirements are:
* docker
* docker-compose
* authorization to build containers
* authorization to forward host ports
* port 8080 open on the host (if you need to use a different port, change docker-compose.yml)

Clone this repo and use docker-compose to bring up the environment:

    git clone https://www.github.com/timquinlan/mirrordemo
    cd mirrordemo
    docker-compose up

Open a 2nd terminal window and test with curl:

    curl http://localhost:8080/test

From the 2nd terminal window use the ab to do some load testing:

    ab -n 100 -c 10 http://localhost:8080/
    
Container layout:

                                       Clients
                                           |
                                           |
                                           |                       --- Mirror1
                                       Apigw --------------|
                                           |                       --- Mirror2
                                  ------------------
                                  |          |         |                            
                               App1  App2  App3                  
<img width="317" alt="image" src="https://user-images.githubusercontent.com/14811185/155863603-f15ce819-3dbb-4642-a071-6d81cf75cfec.png">
