Running Pi-Hole with docker-compose
===================================


    git clone https://github.com/thomasleveil/doco-pihole.git
    cd doco-pihole
    # edit docker-compose.yml to change the value of `ServerIP` so it matches your docker host ip 
    docker-compose up -d
    # then tail the log:
    docker-compose logs -f  # <ctrl>-c to stop tailing the log

In my setup, my docker host IP address is `192.168.1.253`. 
Then set your DNS server IP to `192.168.1.253` on your network interfaces.
And you can access Pi-Hole's admin interface with http://192.168.1.253:8053/admin/

Docker image documentation: https://github.com/diginc/docker-pi-hole
