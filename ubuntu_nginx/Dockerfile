FROM ubuntu:focal

ENV DEBIAN_FRONTEND=noninteractive
RUN apt update -y
RUN apt install -y nginx git

RUN git clone https://github.com/ehszl409/MZ_static_web_template.git 
RUN cp -r MZ_static_web_template/htdocs/* /var/www/html/

CMD ["nginx", "-g", "daemon off;"]


# 포트 열기
EXPOSE 80
