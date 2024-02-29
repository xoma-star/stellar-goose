FROM node:latest
LABEL authors="xoma-star"

# Скачивание или обновление space-terminal-server репозитория
RUN git clone https://github.com/xoma-star/space-terminal-server.git
WORKDIR /space-terminal-server

# Установка node модулей и выполнение yarn serve
RUN yarn install
RUN yarn build

EXPOSE 4000
CMD ["yarn", "serve"]