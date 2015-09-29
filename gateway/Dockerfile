FROM quay.io/ukhomeofficedigital/store-base

ADD build.sh /tmp/build.sh

RUN DOCKER_BUILD=true /tmp/build.sh

WORKDIR /app
EXPOSE 8888
CMD ["/app/bin/boot"]
ADD bin/boot /app/bin/boot
