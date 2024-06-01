FROM --platform=linux/amd64 bellsoft/liberica-openjre-alpine:21
RUN apk --no-cache upgrade busybox libcrypto3 libssl3 && \
    sed -i -r "/^nobody|root/!d" /etc/group && \
    sed -i -r "/^nobody|root/!d" /etc/passwd && \
    rm -rf /sbin/apk /etc/apk /lib/apk /usr/share/apk /var/lib/apk /bin/busybox
USER nobody:nobody
