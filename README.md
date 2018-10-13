\mounts

So, build this docker file into an image, call it 'today', and then
execute the following command.

``docker run -v "$(pwd)"/portal:/app today``

Now you have a container that is using the directory you launched from as its working directory.
In this case, the container is using a directory it refers to as '/app', but that dir is really
the directory './portal', so I think you had better make sure that portal is in your working directory
when you launch the container. The container must be launched from the right place.
