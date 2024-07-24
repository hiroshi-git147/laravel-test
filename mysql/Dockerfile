FROM mysql/mysql-server:8.0
LABEL maintainer="littleheroes <support@littleheroes.jp>"

ARG DOCKERDIR

COPY ./mysql/my.cnf /etc/my.cnf
RUN chmod 644 /etc/my.cnf
