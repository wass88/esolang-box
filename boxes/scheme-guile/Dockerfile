FROM esolang/build-base

RUN apk add guile && \
    rm -rf /var/cache/apk/* /tmp/* && \
    ln -s /bin/script /bin/scheme-guile

COPY script /root/script
