# ICTSC 練習用 cloud-init

ICTSC の過去問の環境を再現できる cloud-init です。  
1 問につき 1 つの yaml ファイルを作成しています。

cloud-init が利用できればどんなツールを使っても大丈夫ですが、[multipass](https://multipass.run/)を推奨しています。

まだまだ不完全なので PR、ISSUE 大歓迎です。

## 使い方

Multipass を用いた環境の作成方法を紹介します。

1. このリポジトリをクローンする

```
https://github.com/KakeruKitahara/ictsc-env.git
cd ictsc-env
```

2. [Multipass 公式サイト](https://multipass.run/install)や[Ubuntu での使い方記事](https://kajindowsxp.com/cloud-init-multipass/)を参考に multipass をインストールする

3. 目的の yaml ファイルを指定し、環境を立ち上げる  
   例:

```
multipass run --name hoge --cloud-init ./2021winter/5l0w-qu3ry.yaml
```

4. 仮想環境に接続する

```
multipass exec hoge bash
```

5. [目的の問題の README](https://github.com/KakeruKitahara/ictsc-env/blob/master/2021winter/5l0w-qu3ry.md)を見て問題にチャレンジ

## 目次

- [ICTSC2021 冬の陣](https://github.com/KakeruKitahara/ictsc-env/tree/master/2021winter)
