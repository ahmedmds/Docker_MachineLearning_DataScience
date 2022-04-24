FROM ubuntu:18.04

WORKDIR /app

COPY requirements.txt ./requirements.txt

RUN apt-get update -y
RUN apt-get install -y python-pip python-dev build-essential
RUN pip install -r requirements.txt

EXPOSE 8501

COPY . /app

ENTRYPOINT ["python"]

CMD ["app.py"]