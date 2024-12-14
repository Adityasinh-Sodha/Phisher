

# Download and import main images

# Operating system
FROM debian:latest
# Main package
FROM python:3



# Working directory
WORKDIR /Phisher/
# Add files 
ADD . /Phisher

# Installing other packages
RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install python3-pip php openssh-client -y
RUN pip3 install -r files/requirements.txt --break-system-packages
RUN apt-get clean

# Main command
CMD ["python3", "Phisher.py", "--noupdate"]

