FROM postgres:18

WORKDIR /app
COPY ./words.sql ./

ENV POSTGRES_HOST_AUTH_METHOD=trust

CMD ["postgres"]