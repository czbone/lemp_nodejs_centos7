# 環境構築プロジェクト
LEMP(Linux,Nginx,MariaDB,PHP)にNodejsを追加した環境をプライベートネットワークに構築します。
WebのルートはNodejsをホスティングし、サブディレクトリでPHPも動作します。

## 構築する環境
- CenOS7
- LEMP
- Nodejs
- Redis


## Webサービスエンドポイント

+ /

Nodejsをホスティングします。

+ /www

PHPをホスティングします。

## 必要な環境

Vagrantが起動する環境が必要です。

## インストール

このレポジトリをダウンロードし、任意の位置に解凍します。


## 起動
vagrantコマンドで環境を起動します。

```
> vagrant up
```

## 初期設定
環境構築後、rootパスワードを設定します。

```
> vagrant ssh
$ sudo su -
$ passwd
```

## サンプルプログラム

サンプルプログラムをダウンロードし配置します。

- https://github.com/czbone/nodejs_php_sample1


## カスタマイズ

デフォルトではプライベートIPの192.168.33.10で起動しますが、Vagrantfileの以下の部分を変更することで任意のIPで起動できます。

```
config.vm.network "private_network", ip: "192.168.33.10"
```
