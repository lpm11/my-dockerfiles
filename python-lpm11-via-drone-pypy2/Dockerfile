FROM bradrydzewski/python:pypy
MAINTAINER lpm11

# Fix rbenv error
ADD rbenv.sh /etc/drone.d/rbenv.sh

# Install packages
RUN . /home/ubuntu/virtualenv/pypy/bin/activate && pip install --use-mirrors fn toolz colorlog
