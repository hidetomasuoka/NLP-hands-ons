# 第2章「自然言語処理」サンプルコード

## 準備

Dockerコンテナを起動し、このディレクトリに移動します。

``` shell
$ cd /webdb100/02
```

## `get_wikipedia.sh`

Wikipediaからデータをダウンロードし、WikiExtractor を実行します。

```shell
$ curl -SL -o jawiki-latest-pages-articles.xml.bz2 https://dumps.wikimedia.org/jawiki/latest/jawiki-latest-pages-articles.xml.bz2
$ git clone https://github.com/attardi/wikiextractor
$ python3.6 wikiextractor/WikiExtractor.py -b 100G -o ./wikipedia_data/extracted ./wikipedia_data/jawiki-latest-pages-articles.xml.bz2
```

## `wikipedia_normalize.py`

Wikipedia のデータを正規化します。

```shell
$ python wikipedia_normalize.py
```

## `wikipedia_wakachi.py`

Wikipedia のデータを分かち書きします。

```shell
$ python wikipedia_wakachi.py
```

このファイルは、<a href="http://creativecommons.org/licenses/by-sa/3.0/">クリエイティブ・コモンズ・表示・継承ライセンス3.0</a>のもとで公表されたウィキペディアの項目<a href="https://ja.wikipedia.org/wiki/%E8%A8%80%E8%AA%9E">「言語」</a>を素材として二次利用しています。
