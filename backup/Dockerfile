
FROM fedora:latest
MAINTAINER Rohith <gambol99@gmail.com>

RUN /usr/bin/dnf install -y tar bzip2 ceph-common python-pip && \
    pip install awscli

ADD https://github.com/michaloo/go-cron/releases/download/v0.0.2/go-cron.tar.gz /tmp/go-cron.tar
RUN tar xvf /tmp/go-cron.tar -C / && \
    rm -f /tmp/go-cron.tar

ADD bin/ceph-backup /usr/bin/ceph-backup
ADD bin/run.sh /run.sh

RUN chmod +x /usr/bin/ceph-backup && \
    chmod +x /run.sh

ENTRYPOINT [ "/run.sh" ]
