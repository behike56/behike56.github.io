---
layout: post
title:  "Clojure Coding - VScode"
date:   2024-06-25 00:00: +0900
categories: jekyll update
tags:
- 開発環境構築
---

## tool

- leiningen
- calva

## プロジェクト作成

`lein new project_name`

## REPLのやり方

### コマンドを選ぶ

`cmd + shift + p`

### REPLの起動

`Calva: Start a Project REPL and onnect (aka Jack-In)` [ctrl + option + c] [ctrl + option + j]

project type:
`leiningen`

### 評価したい関数があるファイルで使用する

`Load/Evaluate Current File and its Requires/Dependencies`　ctrl + option + c Enter

### 関数を評価する

カッコの終わりで実行する。

`Calva: Evaluate Top Level Form (defun)` option + enter
