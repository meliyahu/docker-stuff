FROM nginx:alipine
# Delete local default.conf file
RUN rm /etc/nginx/conf.d/default.conf
# Copy our custom default.conf to nginx configuration
COPY default.conf /etc/nginx/conf.d/

# Remove default index page
RUN rm /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html

# Remove default 50x page
RUN rm /usr/share/nginx/html/50x.html
COPY 50x.html /usr/share/nginx/html
