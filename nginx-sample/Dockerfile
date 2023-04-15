FROM nginx
COPY index.html /usr/share/nginx/html

# Copy the custom NGINX configuration file to the container
# currently this is not working so will be using docker commands to do this manually
# COPY ./default.conf /etc/nginx/conf.d/

# Verify the NGINX configuration
RUN nginx -t
# Containers run nginx with global directives and daemon off
ENTRYPOINT ["nginx", "-g", "daemon off;"]