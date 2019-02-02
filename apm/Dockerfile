ARG APM_VERSION

# https://github.com/elastic/apm-server-docker
FROM docker.elastic.co/apm/apm-server:${APM_VERSION}

COPY apm/config/apm-server.yml /usr/share/apm-server/apm-server.yml
USER root
RUN chown root:apm-server /usr/share/apm-server/apm-server.yml
USER apm-server