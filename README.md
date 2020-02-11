# README

これは Re:VIEW Starter で生成された、Re:VIEW 用プロジェクトです。

* 対象とする Re:VIEW バージョン： 2.5 (これ以外のバージョンだと動作未確認)
* 問い合わせ： Twitter でハッシュタグ「#reviewstarter」つきでツイートしてください。

### Dockerを使う場合

```
$ docker pull kauplan/review2.5    # 3GB 以上ダウンロードするので注意
$ unzip mybook.zip
$ cd mybook/
$ docker run --rm -v $PWD:/work kauplan/review2.5 /bin/bash -c "cd /work; rake pdf"
$ ## または rake docker:pdf でもOK
$ ls mybook.pdf
```