FROM centos:7
RUN yum install epel-release -y
RUN yum install nginx -y
EXPOSE  80
CMD     ["nginx", "-g", "daemon off;"]
#ENTRYPOINT ["nginx", "-g", "daemon off;"]
#CMD     ["sleep", "10"]
#ENTRYPOINT ["sleep", "10"]
ARG     URL
ENV     URL=$URL
COPY    index.html /usr/share/nginx/html/index.html
USER    bin
WORKDIR /opt


