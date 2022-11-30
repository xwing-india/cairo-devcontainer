FROM --platform=linux/amd64 mcr.microsoft.com/devcontainers/python:3.9

ENV PATH="$PATH:~/cairo_venv/bin/activate:/home/vscode/.bashrc'"

RUN apt update && apt install -y libgmp3-dev
RUN pip3 install cairo-lang && pip3 install contextvars

RUN pip3 install cairo-nile

RUN curl -L https://raw.githubusercontent.com/software-mansion/protostar/master/install.sh | bash
