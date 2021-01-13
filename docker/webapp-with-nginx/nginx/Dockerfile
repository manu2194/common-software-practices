# pull official base image
FROM nginx:1.17.9-alpine

# Remove default nginx conf file
RUN rm /etc/nginx/conf.d/default.conf
# Nginx container already has it's own nginx.conf file. Copy a new nginx.conf if you want
# to make any changes to that configuration file.
COPY ./nginx.conf /etc/nginx/nginx.conf

# Make directory for holding SSL certificates and keys
RUN mkdir -p /etc/nginx/ssl
