# HTMLの基本配置を作ろう

## 目次
<!-- toc -->

## HTMLの基本配置を作ろう
htmlの基本配置を作ってみましょう。
何処かに`WebTest`というフォルダをつくり、その中に`index.html`というファイルを作ってみましょう。
内容は以下を入力してください。
```html
<!DOCTYPE html>
<html>
    <head>
        <title>文章生成マシーン</title>
    </head>
    <body>
        <h1>文章生成マシーン</h1>
        <button>生成</button>
        <div>
            <span>あなたは</span>
            <span>耳が</span>
            <span>良い</span>
        </div>
    </body>
</html>
```
今回は、3つの言葉を組み合わせて文章を作るページを作りたいと思います。