FROM python:3.8

WORKDIR /app

COPY ./src/requirements.txt requirements.txt

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

COPY . .