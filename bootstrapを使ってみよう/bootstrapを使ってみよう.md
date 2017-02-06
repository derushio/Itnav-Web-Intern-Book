# bootstarapを使ってみよう

## 目次
<!-- toc -->

## bootstrapを入れよう
ターミナルを起動し、cdコマンドで作業ディレクトリに移動した後に、以下のコマンドを実行する。
```bash
npm init
```
いろいろ出るが、最初の名前以外はエンター連打で問題ない。  
名前は小文字とハイフン`-`で構成される名前にしよう。

以下のコマンドでブートストラップをインストールできます。
```bash
npm install --save bootstrap
```

## HTMLにbootstrapを適用させよう
`<head>`タグに以下を追加しましょう
```html
<link rel="stylesheet" href="./node_modules/bootstrap/dist/css/bootstrap.min.css" />
```

これでbootstrapが使えるようになりました。


## 試しにボタンを変えてみよう
ボタンのタグを以下にしてみましょう。
```html

```
