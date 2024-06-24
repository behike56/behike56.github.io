---
layout: post
title:  "開発環境構築 - asdf clojure"
date:   2024-06-12 00:00:00 +0900
categories: 
tags:
- 開発環境構築
---

## Tool

- asdf
- leiningen

## asdf でJVMをインストールする

{% highlight shell %}

# プラグインをインストール
asdf plugin-add java

# インストール可能なバージョンの確認
asdf list-all java

# インストール
asdf install java openjdk-22.0.1

# 実体の確認
where java
/Users/USERNAME/.asdf/shims/java

asdf which java
/Users/USERNAME/.asdf/installs/java/openjdk-22.0.1/bin/java

# インストールを確認
asdf list java

# グローバルに設定 & shim 再生成
asdf global java openjdk-22.0.1
asdf reshim java

# シェルを再起動 / リロード

# バージョンの確認
java --version

openjdk 22.0.1 2024-04-16
OpenJDK Runtime Environment (build 22.0.1+8-16)
OpenJDK 64-Bit Server VM (build 22.0.1+8-16, mixed mode, sharing)

{% endhighlight %}


## unistall

`asdf uninstall java`
`asdf uninstall java openjdk-22.0.1`

## leiningenのインストール

{% highlight shell %}

brew install leiningen

# 必要な場合、.tool-versionsにバージョンを追記する。

echo "java openjdk-21.0.2" >> /Users/behike56/.tool-versions

{% endhighlight %}

## 参考文献

- [【図解】作業が倍速！pipenvの使い方【Python】]
- [Pythonの開発環境の3つの観点をおさえよう]

[【図解】作業が倍速！pipenvの使い方【Python】]: https://zenn.dev/nekoallergy/articles/py-env-pipenv01
[Pythonの開発環境の3つの観点をおさえよう]: https://zenn.dev/os1ma/articles/935f6e653f1052
