FROM oven/bun:1.0.30

RUN apt-get update  \
    && apt-get install -y git nano \
    && apt-get clean

RUN git clone https://github.com/xoma-star/space-terminal-server.git

WORKDIR ./space-terminal-server

RUN bun install

EXPOSE 3000
CMD ["bun", "serve"]