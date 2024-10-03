# uv-docker

uv + DockerでPython環境を構築するためのテンプレート．


<!-- ## 使用技術

<p style="display: inline">
    <img src="https://img.shields.io/badge/-Python-F2C63C.svg?logo=python&style=for-the-badge">
    <img src="https://img.shields.io/badge/-Docker-1488C6.svg?logo=docker&style=for-the-badge">
</p> -->


## 環境

| 言語・ツール | バージョン |
| ------------ | ---------- |
| Python | 3.12.4 |
| uv | 0.4.17 |


## ディレクトリ構成

```
.
|-- .python-version
|-- Dockerfile
|-- Makefile
|-- README.md
|-- entrypoint.sh
|-- pyproject.toml
`-- uv.lock
```


## セットアップ

```bash
git clone git@github.com:haruto2001/uv-docker.git
```


## 使い方

- イメージののビルド

```bash
make build
```

- コンテナの起動

```bash
make run
```

- linterの実行

```bash
make check
```

- formatterの実行 (diffの表示)

```bash
make format
```

- isortの実行 (diffの表示)

```bash
make isort
```

- コンテナ内でのPythonスクリプトの実行

```bash
uv run python src/hoge.py
```
