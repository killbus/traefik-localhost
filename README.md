# Localhost

a local host using docker-compose and traefik 2.  This is a starting point for other web projects and produces a common mysql database.  

## Installation

1. run `git clone https://github.com/hadamlenz/localhost.git`
2. You need to set up ssl certs for the whoami.localhost and phpmyadmin.localhost`
3. run `docker-compose up -d`
4. in your browser go to https://whoami.localhost/.  you should see a readout of host information
5. in your browser go to 

## Creating TLS certs

1. change directory to the assets folder
2. you need to edit the .conf file so that the `commonName_default` and `alt_names`.  If you want a wildcard cert, edit wildcard-cert.conf
3. run `./make_cert -u {domain}` for a single site cert or `./make_wildcard_cert -u {domain}`.  follow the directions to make the cert
4. trust the cert on your local machine