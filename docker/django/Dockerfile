FROM python:3.7

ENV PYTHONUNBUFFERED 1
RUN apt update
RUN apt install -y nano
RUN mkdir /src
COPY ./src /src
WORKDIR /src

RUN pip install pipenv && pipenv install --system
