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

## 起動
vagrantコマンドで環境を起動します。

```
> vagrant up
```

## 初期設定
rootパスワードを設定します。

```
> vagrant ssh
$ sudo su -
$ passwd
```

## サンプルプログラム


サンプルプログラムをダウンロードし配置します。

https://github.com/czbone/nodejs_php_sample1
