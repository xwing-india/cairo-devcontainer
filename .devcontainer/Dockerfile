FROM --platform=linux/amd64 mcr.microsoft.com/devcontainers/python:3.9

RUN apt update && apt install -y libgmp3-dev
RUN pip3 install cairo-lang && pip3 install contextvars

RUN pip3 install cairo-nile

RUN curl -L https://raw.githubusercontent.com/software-mansion/protostar/master/install.sh | bash
RUN mv /root/.protostar/dist/protostar /opt

ENV PATH="$PATH:~/cairo_venv/bin/activate:/opt/protostar"