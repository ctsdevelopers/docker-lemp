FROM mysql:latest
RUN apt-get update -y && apt-get install -y vim
COPY ./my.cnf /etc/mysql/my.cnf
RUN chmod 644 /etc/mysql/my.cnf
