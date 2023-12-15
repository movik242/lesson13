FROM alpine:latest
ENV NGINX_VERSION nginx:latest
RUN apk update && apk add nginx
EXPOSE 80
EXPOSE 8080
COPY index.html /usr/share/nginx/html/
COPY default.conf /etc/nginx/http.d/
CMD ["nginx", "-g", "daemon off;"] 
