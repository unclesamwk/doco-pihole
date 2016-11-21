Running Pi-Hole with docker-compose
===================================


    git clone https://github.com/thomasleveil/doco-pihole.git
    cd doco-pihole
    # edit docker-compose.yml to change the value of `ServerIP` so it matches your docker host ip 
    docker-compose up -d
    # then tail the log:
    docker-compose logs -f  # <ctrl>-c to stop tailing the log
    
Docker image documentation: https://github.com/diginc/docker-pi-hole
