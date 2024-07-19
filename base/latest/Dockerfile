FROM registry.fedoraproject.org/fedora-minimal:38

LABEL maintainer="Debezium Community"

USER root
RUN microdnf update -y
RUN microdnf install -y java-11-openjdk
RUN microdnf install -y tar
RUN microdnf install -y gzip
RUN microdnf install -y iproute
RUN microdnf install -y findutils
RUN microdnf install -y zip
RUN microdnf clean all
