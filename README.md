# flask-map-dashboard-integration
run a container with python where you can install flask and run an app for dev:
1. docker run -it --name flask-map-dashboard-integration -p 5000:5000 -v ${PWD}:/usr/src/app -w /usr/src/app python:3.7-slim-stretch /bin/bash

To use the docker-compose file that uses the nginx-proxy (previously set up) do the following.
1. add the following to "C:\Windows\System32\drivers\etc\hosts": 127.0.0.1 test.localhost (optional when you dont have a domain name to use in VIRTUAL_HOST, see docker-compose.yml)
2. docker-compose up -d