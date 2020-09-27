FROM python:3.6

WORKDIR  /app

COPY requirement.txt .

RUN apt-get update -y && apt-get install -y openssl swig

RUN pip install --no-cache-dir -r requirement.txt \
    && rm -rf /var/lib/apt/lists/*
