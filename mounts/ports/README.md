### Connect a port on the container to a port on your machine with: -p host:container

`docker run -p 4000:80 friendly`

EXPOSE 80 in the docker file is not needed