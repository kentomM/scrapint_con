# DockerHubのイメージ
FROM python:3.12.4
# ローカルのファイルをコンテナ内にコピー
COPY requirements.txt ${pwd}
# 必要なパッケージをインストール
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# 作業ディレクトリの指定
WORKDIR /workspace

# 環境変数
ENV PYTHONPATH=/workspace/src
