FROM oven/bun
LABEL authors="xoma-star"

RUN apt-get update && \
    apt-get upgrade -y && \
    apt-get install -y git

RUN git clone https://github.com/xoma-star/space-terminal-server.git
WORKDIR /space-terminal-server

RUN bun install --production

EXPOSE 3000
CMD ["bun", "serve"]