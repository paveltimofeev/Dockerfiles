FROM python:3.5-alpine
MAINTAINER Pavel Timofeev <paul.v.timofeev@gmail.com>

ENV BLENDER_VERSION blender-2.78c-linux-glibc219-x86_64

RUN apk upgrade && \
    apk update && \
    apk add wget libxi mesa freetype && \
    pip install PyYAML && \
    mkdir -p /workdir && \
    wget https://www.blend4web.com/blender/release/Blender2.78/$BLENDER_VERSION.tar.bz2 && \
    tar xvf $BLENDER_VERSION.tar.bz2

ENV PATH /$BLENDER_VERSION:$PATH

WORKDIR /workdir
