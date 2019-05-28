FROM python:3.5-slim

RUN mkdir -p /app/

ADD requirements.txt /app/requirements.txt

RUN pip install -r /app/requirements.txt

WORKDIR /app

CMD ["python"]