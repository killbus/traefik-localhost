# Localhost

a local host using docker-compose and traefik 2

## Installation

1. `git clone https://github.com/hadamlenz/localhost.git`
2. You need to set up ssl certs for the whoami.localhost and phpmyadmin.localhost

## Creating TLS certs

1. change directory to the assets folder
2. you need to edit the .conf file so that the `commonName_default` and `alt_names`.  If you want a wildcard cert, edit wildcard-cert.conf
3. run `./make_cert -u {domain}` for a single site cert or `./make_wildcard_cert -u {domain}`.  follow the directions to make the cert
4. trust the cert on your local machine