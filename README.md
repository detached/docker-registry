# Private docker-registry

This repository contains all files for running a private docker registry. You need docker and [docker-compose](https://docs.docker.com/compose/install/) for running these

Place the certificate for the nginx to ./nginx/ssl/docker-registry.crt and ./nginx/ssl/docker-registry.key. You can add user accounts with 

    htpasswd ./nginx/conf/docker-registry.htpasswd $user
    
Replace the %HOST% variable in the nginx.conf to fitt your hostname.

To start up run 

    docker-compose up
