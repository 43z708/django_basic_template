FROM python:3

RUN mkdir /code
WORKDIR /code

COPY .env /
COPY ./src/requirements.txt /code/
RUN pip install --upgrade pip \
    && pip install -r requirements.txt
