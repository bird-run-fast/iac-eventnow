# eventnow

## 概要
ポートフォリオの一環で、架空の webサイトを作成中です。
まずは AWS 環境を IaC に起こしました。
アプリロジックについては、別リポジトリで管理予定です。

## インフラ構成図
![infra_arc](./infra/infra_arc.drawio.svg)

## 使用ツール群

この環境で採用しているツール群です。applyにはこれらがインストール済みであることが前提となります。

* terragrunt
    * terraform を dry に実装するためのラッパーツールです。

* ~~ecspresso~~
    * ~~ECS リソースの作成、デプロイを管理するツールです~~
    * ~~デプロイ頻度 > インフラリソースの頻度だと思うので、管理が分かれていると都合がいいことが多いです~~
    * ~~参考: https://qiita.com/sergicalsix/items/12c2441c08eb9aa311a8~~

## docker

###  実行環境の起動

Bash or PowerShell
```bash
docker compose run app bash
```

