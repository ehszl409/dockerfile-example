FROM ubuntu:focal

ENV DEBIAN_FRONTEND=noninteractive
RUN apt update -y
RUN apt install -y nginx

COPY nginx/sites-available/loadbalancer /etc/nginx/sites-available/loadbalancer
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80
