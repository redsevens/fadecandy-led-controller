FROM resin/raspberrypi3-python:2

RUN apt-get update && apt-get install -yq \
    python-twisted && \
    apt-get clean && rm -rf /var/lib/apt/lists/*

WORKDIR /usr/src/app

COPY ./src/* ./

CMD ["python","artnet-server_fc.py"]
