# Python with scientific packages

FROM bradrydzewski/python:3.3
MAINTAINER lpm11

# Fix rbenv error
ADD rbenv.sh /etc/drone.d/rbenv.sh

# Install dependencies
RUN sudo apt-get update && sudo apt-get install gfortran libblas-dev liblapack-dev libatlas-dev

# Install packages
RUN . /home/ubuntu/virtualenv/python3.3/bin/activate && pip install --use-mirrors cython numpy scipy pandas
