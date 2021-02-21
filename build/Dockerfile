FROM debian:10.7

LABEL maintainer "Dennis Boeckmann <dev@dbck.de>"
LABEL description "Hello world."

ARG TARGETPLATFORM
ARG BUILDPLATFORM

RUN echo "I am running on $BUILDPLATFORM, building for $TARGETPLATFORM"

ENV DEBIAN_FRONTEND noninteractive

COPY root/docker-entrypoint.sh /docker-entrypoint.sh
RUN chmod 755 /docker-entrypoint.sh

ENTRYPOINT ["/docker-entrypoint.sh"]