```
RDSを使うメリット
・冗長化、パッチ適用、インストールの手間が少ない

AWS クラウド推奨構成
https://aws.amazon.com/jp/cdp/

AWS Well Architected FW（★試験対策必須）
https://aws.amazon.com/jp/architecture/well-architected/

■サービスの種類
EC2
EBS(Elastic Block Store) 外付けハードディスク。（OSから直接マウントして使うイメージ）
→DBとか、htmlとかっていう、頻繁にファイルの更新があるものについては、S3ではなくこちらを利用する。
S3 FTPサーバ、静的ファイルを配置すればWebサーバにも。AZが一緒でも、DCはEC2とかとは違う
→CDNとの違いは？
Route53 NDS(portが53だから)
CloudFront CDN(akamai)

オレゴンのサービスはやすい。開発環境だけオレゴンで、本番は東京とかっていう使い分けもできる。


水 テストNGの認識合わせ＋インストールパッケージとか整理（コミット）
木 バッチ打ち合わせ＋テスト仕様書とパラ設なおし
金 バッチ打ち合わせ＋本番用のyumインストール

来週
月　本番インストール＋テスト性能

今日
バッチのフローを考える
Dockerの永続化とRedmineのオンラインバックアップについて
Postgresqlのバックアップ
```
