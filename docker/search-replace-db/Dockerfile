FROM php:alpine
RUN apk add git bash
RUN docker-php-ext-install -j$(nproc) pdo pdo_mysql
RUN git clone https://github.com/interconnectit/Search-Replace-DB && git clone https://github.com/vishnubob/wait-for-it
COPY run.sh .
CMD sh run.sh