# Sim_Web
A simple HTML-based Docker image with a .tar file as the HTML template and a Dockerfile to create the corresponding Docker image.

Steps:
1) docker build -t nanoimg .  # to build image. -t is the option to give name. nanoimg is the name of the image. "." shows the files are the same dir.
2) docker run -d --name nanowebsite -p 9080:80 nanoimg  # -d for running the image in the background
3) docker login  # to login to DockerHub
4) Build the image again with this name: DockerHubAccountName/ImageName
5) docker push DockerHubAccountName/ImageName:TAG
6) docker pull DockerHubAccountName/ImageName:TAG. # now everybody can use this command to install the docker image!


