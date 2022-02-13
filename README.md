# ReverseProxy

This is the setup of a simple reverse proxy with https (self signed) and basic auth that I use together with private projects. (e.g. [https://github.com/HaraldKangSchroeder/DigitalInformationAdministrator](https://github.com/HaraldKangSchroeder/DigitalInformationAdministrator))

## Setup
1. The application comes along with Docker, specifically docker-compose, so you need to install those first - see [https://docs.docker.com/compose/install/](https://docs.docker.com/compose/install/). You also need an account on Docker Hub ([https://hub.docker.com/](https://hub.docker.com/)).
2. Create a .env file, paste the content of the .sample-env file in there and set the environment variables accordingly. These values are used to generate a self signed certificate and utilized for basic authentication.
3. Create a nginx.conf file, paste the content of the sample-nginx.conf file in there and set your routing as desired (example routes are already given).
4. Execute `docker-compose up` to start the reverse proxy (append -d flag to start in detached mode).
