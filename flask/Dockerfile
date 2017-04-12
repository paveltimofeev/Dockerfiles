FROM Python:3.5-alpine

ENV ver 1

RUN apk add --no-cache --update \
          curl \
  && pip install --upgrade pip \
  && pip install --no-cache-dir \
          virtualenv \
          Flask \
  && rm -rf /var/cache/apk/*
  
