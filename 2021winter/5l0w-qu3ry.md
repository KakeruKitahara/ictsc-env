# 5l0w qu3ry

cloud-init ファイル  
https://github.com/KakeruKitahara/ictsc-env/blob/master/2021winter/5l0w-qu3ry.yaml

元サイトと解答  
https://blog.icttoracon.net/2022/03/04/5l0w-qu3ry/

## 概要

カテゴリをフィルタリングするシステムを構築したが初回取得時になぜか遅いので検証環境を構築した。  
原因を特定して速くして欲しい。

## 前提条件

- 初回取得時を再現するためにキャッシュをオフにしている、そのためキャッシュを使う様に設定を書き換える行為を禁止とする。
- `/var/www/html/index.php` の変更禁止。

## 初期状態

`curl localhost` で取得しようとするがレスポンスが遅い。

## 終了状態

1300ms (1.3 秒) 以内で取得出来るようにする。
