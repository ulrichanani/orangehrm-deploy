FROM httpd:latest

# Copy apache vhost file to proxy php requests to php-fpm container
COPY vhost.conf /usr/local/apache2/conf/default.apache.conf
RUN echo "Include /usr/local/apache2/conf/default.apache.conf" \
    >> /usr/local/apache2/conf/httpd.conf

WORKDIR /var/www/html/

RUN chmod 777 -R .