FROM nginx:1.26.0-bookworm
COPY sites-enabled/ /etc/nginx/sites-enabled/
RUN rm -v /etc/nginx/conf.d/default.conf
RUN rm -v /etc/nginx/nginx.conf
COPY conf/nginx.conf /etc/nginx/nginx.conf
COPY www/ /var/www/
EXPOSE 80 443
