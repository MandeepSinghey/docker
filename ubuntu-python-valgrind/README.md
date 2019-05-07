########################
# In current directory build a docker image
########################

# create a image name "ubuntu" on local machine using the Dockerfile in current directory
# -t, --tag =  Name and optionally a tag in the ‘name:tag’ format
docker build -t ubuntu  .
