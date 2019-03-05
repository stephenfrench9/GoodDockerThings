
So, build this docker file into an image

``docker build . -t today``

Run the image with the following command

``docker run -itv $(pwd):/created_from_commandline today``

When using the -v flag, you really have to specify full addresses, relative addresses are not ok. The -v flag will create a new directory in the image. Also, when you set the working directory in the Dockerfile, a new directory is created. 

open question: which of these dirs is created first, and can they collide with each other? Do they happen after the container is running? Or during some pre-run build time?
