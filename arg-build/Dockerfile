FROM debian

LABEL authors="Daniel"

ARG TEST=local_test

ENV ARG1=${TEST}

# docker image inspect --format="{{index .Config.Labels \"authors\"}}" debian:test