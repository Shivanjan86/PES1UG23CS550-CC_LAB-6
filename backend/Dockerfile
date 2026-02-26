FROM ubuntu:22.04

RUN apt-get update --allow-insecure-repositories && \
    apt-get install -y --allow-unauthenticated g++

WORKDIR /app

COPY app.cpp .

RUN g++ app.cpp -o app

EXPOSE 8080

CMD ["./app"]
