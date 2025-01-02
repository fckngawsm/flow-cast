FROM postgres:16.4-alpine3.20

WORKDIR /app

COPY ./init /docker-entrypoint-initdb.d/
COPY ./dump.sql /dumps/dump.sql

# Устанавливаем права на выполнение для всех скриптов
RUN chmod -R +x /docker-entrypoint-initdb.d/
