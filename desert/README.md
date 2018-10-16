Launch a jupyter notebook container

`docker run -d -t cloudwhale jupyter/minimal-notebook`

Find the ports the notebook is being publish too: (its prolly 8888)

`docker inspect cloudwhale`

Find the working directory of the container:

`docker exec cloudwhale pwd`

Shut down the notebook. Start the container again. This time, connect your host port to the containers port

`docker run -d -p 8888:8888 -v $(pwd):/home/jovyan cloudwhale`

