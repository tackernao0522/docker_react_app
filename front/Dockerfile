FROM node:16.13.1-alpine

ARG WORKDIR

ENV HOME=/${WORKDIR}

WORKDIR ${HOME}

# ローカル上のpackageをコンテナにコピーしてインストールする
COPY package*.json ./
RUN npm install


# コンテナにNextプロジェクトをコピー
COPY . ./
