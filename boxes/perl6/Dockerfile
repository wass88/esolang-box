FROM esolang/build-base

RUN apk update && \
    apk add ca-certificates wget && \
    update-ca-certificates    
RUN apk add --update perl && \
    cd /tmp && \
    wget https://rakudo.perl6.org/downloads/star/rakudo-star-2019.03.tar.gz && \
    tar xfz rakudo-star-2019.03.tar.gz && \
    cd rakudo-star-2019.03 && \
    perl Configure.pl --gen-moar --make-install
 RUN rm -rf /var/cache/apk/*  && \
     ln -s /bin/script /bin/perl6

COPY script /root/script
