# Jup3Docker
Docker to run Jupyter with Python3

This folder contains the files needed to create a Python version3 Jupyter notebook environment. The requirements files contains my own package that I have used on Sherlock.

I use a bash script to run the docker afterwards

To run the docker:

Go into the Jup3Docker folder and then at the prompt:

$ DOCKER_NAME="nadeemjup3"; docker build -t $DOCKER_NAME . # This will build the container with the name nadeemjup3
$ source python3_docker_no.sh

An alias has been created (Py3_Nbook) that will start the Jupyter docker. Note that inside the bash file, we have hardcoded (for now) the volumes that will need to be mounted. These can be changed as per the user. We will put a much better way in the future.

$ Py3_Nbook

The Jupyter notebook can be accessed, for e.g. on Sherlock at http://sherlock.sdp.kat.ac.za:8891/

NB: The port 8891 is hardcoded for now inside the python3_docker_no.sh

