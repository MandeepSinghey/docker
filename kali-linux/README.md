# In current directory build a docker image

### Create a image name "kali-linux" on local machine 

### https://medium.com/@airman604/kali-linux-dockerfile-afb69f1a08db

### Using the Dockerfile in current directory

### -t, --tag =  Name and optionally a tag in the ‘name:tag’ format

<font color='red'>
    Note: Things which need to be installed permanently need to be added to this file, to be installed on image.
</font>

## Build
docker build -t kali-linux  .

## Run
docker run -t -i kali-linux

## Docker Images

https://docs.docker.com/engine/docker-overview/

An image is a read-only template with instructions for creating a Docker container. Often, an image is based on another image, with some additional customization. For example, you may build an image which is based on the ubuntu image, but installs the Apache web server and your application, as well as the configuration details needed to make your application run.

You might create your own images or you might only use those created by others and published in a registry. To build your own image, you create a Dockerfile with a simple syntax for defining the steps needed to create the image and run it. Each instruction in a Dockerfile creates a layer in the image. When you change the Dockerfile and rebuild the image, only those layers which have changed are rebuilt. This is part of what makes images so lightweight, small, and fast, when compared to other virtualization technologies.