ARG FROM_IMAGE
FROM $FROM_IMAGE

LABEL maintainer "Dennis Boeckmann <dev@dbck.de>"
LABEL description "Hello world."

ENV DEBIAN_FRONTEND noninteractive

COPY root/docker-entrypoint.sh /docker-entrypoint.sh
RUN chmod 755 /docker-entrypoint.sh

ENTRYPOINT ["/docker-entrypoint.sh"]