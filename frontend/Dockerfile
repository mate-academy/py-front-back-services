FROM python:3.11

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

RUN apt-get update && apt-get install -y graphviz graphviz-dev netcat-openbsd
RUN pip install --upgrade pip

WORKDIR /code

COPY ./requirements.txt /code/requirements.txt

RUN pip install -r /code/requirements.txt

COPY . /code
COPY entrypoint_frontend.sh /entrypoint_frontend.sh

RUN chmod +x /entrypoint_frontend.sh
