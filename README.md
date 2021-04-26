# 構築環境
LEMP(Linux,Nginx,MySQL,PHP)にNodejsを追加した環境をプライベートネットワークに構築します。
WebのルートはNodejsをホスティングし、サブディレクトリでPHPも動作します。

## ベースOS
- CenOS7

## Webサービスエンドポイント

+ /

Nodejsをホスティングします。

+ /www

PHPをホスティングします。

## 実行方法
vagrantコマンドで環境を起動します。

$ vagrant up

