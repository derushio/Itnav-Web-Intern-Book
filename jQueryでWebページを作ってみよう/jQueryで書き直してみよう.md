# jQueryで書き直してみよう

## 目次
<!-- toc -->

## HTMLにjQueryの読み込みを書いてみよう
HTMLのindex.jsを読み込んでいる前に以下のコードを追加しましょう。  
これでjQueryを利用することができるようになります。
```html
<script src="https://code.jquery.com/jquery-3.1.1.min.js"></script>
```

## buttonのonClickを外そう
buttonタグを以下の様に書き換えましょう
```html
<button id="generate">生成</button>
```

## JS側の参照をjQueryにしてみましょう。
jQueryでは、以下のような記述が可能になります。
```javascript
var textmap = [
    ["私は", "あなたは", "あの人は"],
    ["耳が", "目が", "鼻が"],
    ["良い", "悪い", "普通"]
];

function randIndex(array) {
    return Math.floor(Math.random() * array.length);
}

$(function() {
    $("#generate").on("click", function() {
        $("#text1").text(textmap[0][randIndex(textmap[0])]);
        $("#text2").text(textmap[1][randIndex(textmap[1])]);
        $("#text3").text(textmap[2][randIndex(textmap[2])]);
    });
});
```
`$(function(){})`でHTMLを読み込みこんだ時に動作させるスクリプトを書くことができます。  
`$("#id")`でidからエレメントを取得することができます。  
また、取得したエレメントでjQueryの便利な機能を使うことができます。