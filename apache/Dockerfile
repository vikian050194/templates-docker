FROM httpd:alpine
ENV PORT=80
EXPOSE ${PORT}
WORKDIR /usr/local/apache2/htdocs
# CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
ENTRYPOINT ["/usr/sbin/apache2", "-D", "FOREGROUND"]
COPY ./febe/hostname.conf /usr/local/apache2/conf/httpd.confs
# COPY index.html index.css index.js favicon.svg ./