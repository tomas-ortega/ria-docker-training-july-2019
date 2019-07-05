FROM ubuntu:18.10

RUN apt-get update
RUN apt-get install nginx -y

RUN useradd pakito

#USER pakito

ENV DATABASE_IP=80.54.23.0
ENV DATABASE_NAME=moneytransfer

EXPOSE 80 443

RUN echo '<marquee>Hello From Ria!!!</marquee>' \
    > /var/www/html/index.html

COPY my-file-data.txt /etc

WORKDIR /etc

#ENTRYPOINT [ "nginx","-g","daemon off;" ]

VOLUME [ "/pakito-volume" ]

CMD ["nginx","-g","daemon off;"]