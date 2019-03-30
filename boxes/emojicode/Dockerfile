FROM esolang/ubuntu-base

ENV BUILD_PACKAGES="rsync ncurses" \
    RUNTIME_PACKAGES="libc6-compat" \
    TERM="dumb"

RUN apt-get install -y rsync && \
    cd /tmp && \
    curl -m $TIMEOUT https://github.com/emojicode/emojicode/releases/download/v0.9/Emojicode-0.9.0-Linux-x86_64.tar.gz -LO && \
    tar xzf Emojicode-0.9.0-Linux-x86_64.tar.gz  && \
    cd Emojicode-0.9.0-Linux-x86_64 && \
    mkdir -p ~/Emojicode/bin && \
    (yes | ./install.sh ~/Emojicode/bin ~/Emojicode/Emojipackages) && \
     ln -s /bin/script /bin/emojicode

ENV EMOJICODE_PACKAGES_PATH /root/Emojicode/Emojipackages

COPY script /root/script
