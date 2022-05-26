From storkmax/nginx-phpfpm7

RUN apk update && \
    apk add -f openssh-server openssh-client docker-cli vim python3  make git diffutils && \
    ssh-keygen -A && passwd -d root && \
    rm -rf /var/cache/apk/*

WORKDIR /root
CMD ["/usr/sbin/sshd", "-D", "-p22"]
