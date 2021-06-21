FROM nginx:alpine
ENV PORT=80
EXPOSE ${PORT}
WORKDIR /usr/share/nginx/html
# CMD ["nginx", "-g", "daemon off;"]
ENTRYPOINT ["nginx", "-g", "daemon off;"]
COPY ./febe/hostname.conf /etc/nginx/conf.d/default.conf
# COPY index.html index.css index.js favicon.svg ./