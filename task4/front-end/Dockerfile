# Use the latest Nginx as the base image
FROM nginx:latest

# Copy the softy-pinko-front-end directory to the Docker image
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx config file to the Docker image
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000 for Nginx
EXPOSE 9000
