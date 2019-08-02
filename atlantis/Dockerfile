FROM alpine:3.7

RUN apk add --no-cache --virtual .build-deps gcc python3-dev musl-dev libffi-dev openssl-dev make && \
    apk add --no-cache --update python3 && \
    pip3 install --upgrade pip setuptools

RUN apk add git

RUN mkdir -p /app/

ADD requirements.txt /app/requirements.txt

RUN pip install -r /app/requirements.txt

RUN apk del .build-deps

WORKDIR /app

ENTRYPOINT ["python3"]