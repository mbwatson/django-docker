FROM python:3.6

ENV PYTHONUNBUFFERED 1

RUN mkdir /src
COPY ./src /src
WORKDIR /src

RUN pip install pipenv && pipenv install --system
