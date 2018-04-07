
# 第2章「自然言語処理」サンプルコード

## 準備

Dockerコンテナを起動し、このディレクトリに移動します。

```
$ cd /webdb100/02
```

## `get_wikipedia.sh`

Wikipediaからデータをダウンロードし、WikiExtractor を実行します。

```
$ ./get_wikipedia.sh
```

## `mecab.py`

Python から MeCab を実行します。

```
$ python mecab.py
```

## `cabocha.py`

Python から CaboCha を実行します。

```
$ python cabocha.py
```

## `content_word.py`

内容語を出力します。

```
$ python content_word.py
```

## `wikipedia_normalize.py`

Wikipedia のデータを正規化します。

```
$ python wikipedia_normalize.py
```

## `wikipedia_wakachi.py`

Wikipedia のデータを分かち書きします。

```
$ python wikipedia_wakachi.py
```

このファイルは、<a href="http://creativecommons.org/licenses/by-sa/3.0/">クリエイティブ・コモンズ・表示・継承ライセンス3.0</a>のもとで公表されたウィキペディアの項目<a href="https://ja.wikipedia.org/wiki/%E8%A8%80%E8%AA%9E">「言語」</a>を素材として二次利用しています。
