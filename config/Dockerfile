
FROM quay.io/ukhomeofficedigital/store-base
MAINTAINER Rohith <gambol99@gmail.com>

ADD config/rbd /bin/rbd
ADD config/rbd-image /bin/rbd-image
ADD config/ceph /bin/ceph
ADD config/rados /bin/rados
ADD config/startup /bin/startup

RUN chmod +x /bin/startup

CMD [ "/bin/startup" ]
