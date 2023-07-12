# Use the latest Ubuntu as the base image
FROM ubuntu:latest

# Update APT package lists
RUN apt-get update

# Upgrade currently installed software
RUN apt-get upgrade -y

# Set the working directory
WORKDIR /app

# Add an entrypoint script
COPY entrypoint.sh /app/entrypoint.sh
RUN chmod +x /app/entrypoint.sh

# Set the entrypoint command
ENTRYPOINT ["/app/entrypoint.sh"]

# run the docker image in container
CMD ["echo", "Hello, World!"]