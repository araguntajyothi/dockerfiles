FROM almalinux:latest

LABEL AUTHOR="Jyothi A"\
      COURSE="DOCKER"\
      DURATION="25 hrs"

ENV NAME="Jyothi A"\
    EMAIL="Jyothi@gmail.com"\
    COURSE="DOCKER"

EXPOSE 8080/tcp

RUN yum install nginx -yum

CMD ["nginx", "-g", "daemon off;"]