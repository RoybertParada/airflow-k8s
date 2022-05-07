FROM python:3.7-alpine

RUN apk update
RUN pip install --upgrade pip

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

WORKDIR /app

ENV PYTHONPATH "${PYTHONPATH}:/app/"

COPY . .