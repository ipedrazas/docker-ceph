FROM quay.io/ukhomeofficedigital/store-base

WORKDIR /app

ADD bin/boot /app/bin/boot
ADD bin/ceph /app/bin/ceph
ADD bin/rados /app/bin/rados
ADD bin/rbd /app/bin/rbd
ADD bin/rbd-image /app/bin/rbd-image
ADD bin/startup /app/bin/startup
RUN chmod +x /app/bin/startup

CMD ["/app/bin/startup"]
