# Use the latest Ubuntu as the base image
FROM ubuntu:latest

# Update APT package lists
RUN apt-get update

# Upgrade currently installed software
RUN apt-get upgrade -y

# Install Python3, Python3-pip, and Flask
RUN apt-get install -y python3 python3-pip
RUN pip3 install flask

# Set the working directory
WORKDIR /app

# Copy the Python file to the Docker image
COPY api.py /app/api.py

# Set the entrypoint command to run the Flask server
ENTRYPOINT ["python3", "api.py"]

# Expose port 5252 for the Flask server
EXPOSE 5252
