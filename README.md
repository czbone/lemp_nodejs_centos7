# 構築環境
LEMP(Linux,Nginx,MySQL,PHP)にNodejsを追加した環境をローカルネットワークに構築します。
WebのルートはNodejsをホスティングし、サブディレクトリでPHPも動作します。

# ベースOS
- CenOS7

# エンドポイント

+ /

Nodejsサービスをホスティングします。

+ /www

PHPサービスをホスティングします。

## 実行方法
vagrantコマンドで環境を起動します。

$ vagrant up

