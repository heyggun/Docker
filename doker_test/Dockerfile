FROM python:3.10

RUN apt-get update -y && \
    apt-get install --yes gnupg gnupg2 gnupg1 curl g++


# install Python requirements
COPY requirements.txt /tmp/requirements.txt
RUN pip install --upgrade pip && \
    pip install -r /tmp/requirements.txt --quiet --no-cache-dir &&  \
    rm -r /tmp/requirements.txt