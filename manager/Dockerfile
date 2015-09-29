FROM quay.io/UKHomeOffice/store-base

ADD https://github.com/gambol99/rbd-fence/releases/download/0.0.4/rbd-manager_0.0.4_linux_x86_64.gz /bin/rbd-manager.gz
RUN gunzip /bin/rbd-manager.gz && \
    chmod +x /bin/rbd-manager

ENTRYPOINT ["/bin/rbd-manager"]
