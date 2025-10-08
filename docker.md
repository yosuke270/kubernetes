# Docker

## はじめに
dockerのサービスはdocker clientとdemonで構成されている
clientは、ユーザからのdockerコマンドを受け取るインターフェースの役割
demonはバックグラウンドの仕組みで、clientから送られてきたコマンドから実際にコンテナを作成したりする役割。

## 流れ

1. docker pullでimageを取得
2. docker imageでpullできているか確認
3. docker runでimagesからコンテナを作成、起動
4. docker stopでコンテナを停止
5. 一度作ったコンテナを再び動かすにはdocker start
6. 一度作ったコンテナを確認したい時はdocker ps -a
7. docker に直接入って作業するにはdocker exec -it <コンテナID>　/bin/bash
