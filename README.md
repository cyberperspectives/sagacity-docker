# sagacity-docker
Repository to contain files needed to create a Docker dev environment for Sagacity.
To use this simply download or clone this repo to your local path, then download or clone https://github.com/cyberperspectives/sagacity in a subdirectory.  Then opening a terminal/command prompt, navigate to this directory and type `docker-compose up` to create and start the required docker containers.

sagacity
  - docker-compose.yml
  - sagacity
    - Dockerfile
    - {code}  

The last thing to do is navigate to "http://localhost" to view the setup.  Docker will create a MySQL 5.7 server with the root password `password`, so during setup you will use "db" as the database hostname.  If you want to change the password, open the docker-compose.yml file and change the line `MYSQL_ROOT_PASSWORD=password` with the password you want to use.