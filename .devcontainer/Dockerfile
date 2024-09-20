# ベースイメージの指定
FROM mcr.microsoft.com/devcontainers/typescript-node:18

# 作業ディレクトリの設定
WORKDIR /workspaces/

# 必要なパッケージをインストール（必要に応じて）
RUN apt-get update && apt-get install -y \
    curl \
    sudo \
    unzip \
    make \
    git \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

# COPY create-awscli-environment.sh /tmp/

# RUN /bin/bash -e /tmp/create-awscli-environment.sh

# ポートのエクスポート
EXPOSE 4321
