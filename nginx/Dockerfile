From amazonlinux:2016.09

RUN set -x && \
    yum --enablerepo=amzn-main clean metadata && \
    yum install -y nginx && \
    touch /etc/sysconfig/network

EXPOSE 80

STOPSIGNAL SIGTERM

CMD ["nginx", "-g", "daemon off;"]
