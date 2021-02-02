# Re:VIEW Template

このリポジトリはRe:VIEW用の書籍テンプレートです。Re:VIEWバージョン5.0に対応します。

このリポジトリは、[TechBookster様のテンプレート](https://github.com/TechBooster/ReVIEW-Template)をforkしてdevcontainer化しています。

## 必要な環境

- Visual Studio Code（以下 VS Code）
- Remote Development Extension

## このテンプレートの使い方は？

VS Codeを用いて、devcontainerで開きます。

その後、ターミナルを開いて次のコマンドを実行します。

```shell
# npm install
```


### Re:VIEWコマンドでPDFを出力する

セットアップが完了していれば `npm run pdf` のかわりに
```
$ cd ReVIEW-Template/articles
$ rake pdf
```

または

```
$ cd ReVIEW-Template/articles
$ review-pdfmaker config.yml
```

でも生成できます。

## EPUB・Webページ・テキストの出力

PDF以外に、EPUB・Webページ・テキストを出力することもできます。

### EPUBを出力する

```
$ npm run epub
```

または

```
$ cd ReVIEW-Template/articles
$ rake epub
```

または

```
$ cd ReVIEW-Template/articles
$ review-epubmaker config.yml
```

### Webページを出力する（webrootフォルダー）

```
$ npm run web
```

または

```
$ cd ReVIEW-Template/articles
$ rake web
```

または

```
$ cd ReVIEW-Template/articles
$ review-webmaker config.yml
```

### テキストファイルを出力する

```
$ npm run text
```

または

```
$ cd ReVIEW-Template/articles
$ rake text
```

または

```
$ cd ReVIEW-Template/articles
$ review-textmaker config.yml
```

## 権利

Fork元のライセンスを継承し、MITライセンスとします。

 * 設定ファイル、テンプレートなど制作環境（techbooster-doujin-base.styなど）はMITライセンスです
   * 再配布などMITライセンスで定める範囲で権利者表記をおねがいします
   * 本設定を使って生成した書籍は現段階のRe:VIEWではソフトウェアたりえません。したがってライセンスは発生しません（あとがきなどへの表記はあると嬉しいものの生成物での表記は不要です）
 * articles/styにあるファイルには以下のライセンスが適用されています。
   * review-jsbook.cls, review-base.sty, review-style.sty, review-custom.sty: MIT License
   * jumoline.sty: The LaTeX Project Public License
   * plistings.sty: MIT License
   * gentombow.sty: BSD License
   * jsbook.cls: BSD License
