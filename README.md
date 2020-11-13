# Localhost

a local host using docker-compose and traefik 2.  This is a starting point for other web projects and produces a common mysql database.  

## Installation

1. You need to set up ssl certs for the 127.0.0.1`
2. run `docker-compose up -d`
3. in your browser go to https://127.0.0.1/. you should see a readout of host information
4. in your browser go to 

## Creating TLS certs

1. install tools: https://github.com/devilbox/cert-gen
2. follow that guide to generate ca and cert.