# nlp-preprcessing
日本語の自然言語処理におけるデータ前処理の基本のき

## 動作確認環境
- CentOS Linux 7
- Windows 10 ver1909
- macOS Catalina ver10.15.7

## 使用言語
- python 3.7.6

## 使用ライブラリ
- neologdn 0.4
- emoji 0.6.0
- mecab-python3 1.0.1

## 事前準備
上記のライブラリが入っていない場合、インストールします。

`$ pip install neologdn`
<br>
`$ pip install emoji`
<br>
`$ pip install mecab-python3`

但し、MeCabに関してはこれだけでは動作しません。更に下記の手順に従って、インストールを行ってください。<br>
[MeCab: Yet Another Part-of-Speech and Morphological Analyzer](https://taku910.github.io/mecab/)

管理者権限がない場合、下記の記事が非常に役に立ちます。<br>
[sudoが使えないマシンでmecabを使うまでの備忘録](https://qiita.com/kadotami/items/57bc2fbb5132b79c7efe)

## 使用方法
`preprocessing.py`内の`pre_processing`関数に対し、前処理を行いたい文を引数として与えてください。
