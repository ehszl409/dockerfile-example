FROM ubuntu:focal

ENV DEBIAN_FRONTEND=noninteractive
RUN apt update -y
RUN apt install -y apache2 git

RUN git clone https://github.com/ehszl409/MZ_static_web_template.git 
RUN cp -r MZ_static_web_template/htdocs/* /var/www/html/

# Apache2 서비스 시작
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]

# 포트 열기
EXPOSE 80
