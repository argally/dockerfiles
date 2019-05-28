FROM amandagalligan/python_data:1.1

RUN mkdir -p /app/

ADD requirements.txt /app/requirements.txt

RUN pip install -r /app/requirements.txt

WORKDIR /app

ENTRYPOINT ["python"]