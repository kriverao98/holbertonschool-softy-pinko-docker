# Use the latest version of Nginx
FROM nginx:latest

# Copy front-end files to the Nginx web root
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy custom Nginx configuration file
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose the port
EXPOSE 9000
