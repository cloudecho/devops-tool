FROM alpine:3.15.4
LABEL maintainer="Yong Ma <simple163@yahoo.com>"

RUN apk add openssh-client
RUN addgroup -g 1000 -S user && \
  adduser -u 1000 -S user -G user && \
  mkdir -p /home/user/.ssh && \
  chown -R user:user /home/user/.ssh

USER user
