# javaScript練習問題① 説明
この問題ではJavaScriptについての「説明」をしてもらいます。
レビューの際には、内容だけでなく、「説明力」という観点でもチェックしているので、誰がみてもわかるような文章で記載してください。

```
悪い例：
- 問題：変数とは何か説明してください。
- 回答：箱。

良い例：
- 問題：変数とは何か説明してください。
- 回答：「変数」とは、データを一時的に保存するための容器のようなものです。変数名はletで始まり、その後に名前が続きます（例：let variableName）。
```

## 「変数」を使用する上での下記3つのメリットについて、説明してください。
- 再利用性: 中身を書き換えるだけで同じ変数を何度も使えるので再利用性が高い
- 可読性の向上: 変数名は自由に名づけることができ、適正な変数名を使用すればどのような値を代入するためのものなのかわかりやすくすることができるため、可読性の向上につながる
- 保守性の向上: 変数を使用することによって、どこにどのような値を代入しているかわかりやすくなり、保守しやすくなることに繋がる

## 下記のデータ型についてそれぞれ説明をしてください。
- 整数型（Number）: 正負の整数を表すデータ型で、符号をつけることが可能。
- 浮動小数点型（Float）: 小数点以下の値を持つ数字を表すデータ型で、指数表現も使用可能。
- 文字列型（String）: 文字を表すデータ型で、''や""を使用することで指定可能。
- ブーリアン型（Boolean）: 与えられた値を「true」か「false」の二通りで表すデータ型。

## テンプレートリテラルの特徴を説明してください。
-値をバッククォートで囲んだものでリテラル（ソースコード上の文字列や数字）の記載形式。テンプレートリテラル内で使いたい式や変数を${}で囲むことで埋め込むことができる。

## 配列とオブジェクトの違いについて「インデックス」「キー」「バリュー」「プロパティー」という単語を使用して説明してください。
-配列はキーがインデックス番号として自動的に取得され、値（バリュー）のみに名前を付けられるのに対し、オブジェクトはキーとバリューがセットになったもので、プロパティを指定してデータを参照する。または配列には順序があるが、オブジェクトにはない。

## Q4で使用したplayerListという変数は「配列」か「オブジェクト」どちらか、また、なぜそう言えるのかを説明してください。
-オブジェクト:波括弧で囲ってあり、キーとバリューがそれぞれ指定されているから。

## 関数について、「関数」「引数」「返り値」という単語を使用して説明してください。
- 関数とは、様々な処理を1つにまとめて名前をつけることができるもので、引数を指定することによって関数内で自由に扱えるようになり、returnを指定することによって返り値が設定され処理内容の結果を普通の値として出力できるようになる。

## 関数とメソッドの違いは何か説明してください。
- 関数は複数の処理をまとめた記述で、メソッドはオブジェクトの操作を定義したもの。

## 下記コードを実行し、「鈴木さん、こんにちは」が出力されない理由を説明してください。
```
function hello(name) {
  console.log("田中さん、こんにちは");
  return `${name}さん、こんにちは`;
  console.log("鈴木さん、こんにちは");
}

let name = '佐藤';
console.log(hello(name));
```
- returnが記述されている時点で関数内の処理が返されているため、その後に記述されているconsole.log()に辿り着くことがないから。