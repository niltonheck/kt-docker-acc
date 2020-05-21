FROM ubuntu:latest

RUN apt-get update && apt-get upgrade -y

RUN apt-get install -y curl

RUN curl -sL https://deb.nodesource.com/setup_12.x | bash -

RUN apt-get install -y nodejs

COPY ./src/ /app/

EXPOSE 3000

CMD ["node","/app/app.js"]