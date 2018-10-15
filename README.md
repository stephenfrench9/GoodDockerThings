\mounts

So, build this docker file into an image

``docker build . -t today``

Run the image with the following command

``docker run -v "$(pwd)"/portal:/app today``

The image is going to run whatever you have placed in /portal and called app.py. It will use /portal/ as its working directory.
Note: The image really expects to find something called "app.py" in whatever directory you desginate as its working directory.
