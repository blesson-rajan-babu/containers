FROM --platform=linux/amd64 bellsoft/liberica-runtime-container:jre-21-slim-glibc
RUN sed -i -r "/^nobody|root/!d" /etc/group && \
    sed -i -r "/^nobody|root/!d" /etc/passwd && \
    rm -rf /bin/busybox
USER nobody:nobody
