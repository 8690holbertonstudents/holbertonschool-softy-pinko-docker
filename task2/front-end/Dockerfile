#Use NGINX open-source web server
FROM nginx:latest
# Copy front-end directory to docker /var/... directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end
# Copy NGINX config file to docker /etc/... directory
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
# Expose port 9000
EXPOSE 9000
# Start NGINX with container
CMD ["nginx", "-g", "daemon off;"]
