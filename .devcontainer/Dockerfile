FROM python:3.10-slim-buster
RUN apt-get update && apt-get install -y \
    curl \
    git

ENV PYTHONDONTWRITEBYTECODE 1 \
    PYTHONUNBUFFERED 1 \
    POETRY_VERSION=1.1.14

RUN curl -sSL https://raw.githubusercontent.com/python-poetry/poetry/master/get-poetry.py | python
ENV PATH="${PATH}:/root/.poetry/bin"