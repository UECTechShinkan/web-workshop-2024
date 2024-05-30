# 3-1. style 属性を使ってみよう

ここでは、[前回](../../part-2/handouts/1_what_is_html.md) の内容で少しだけ出てきた、`style` 属性について学びます。

## `style` 属性

![<p>Hello World!</p>(<p>が開始タグ、Hello World!がコンテンツ、</p>が終了タグ)](../../part-2/handouts/images/1_element_with_attr.png)

このように書くことで、特定の HTML 要素に直接スタイルを適用することができます。

この例では、文字の色（`color`） に対して、赤色（`red`）を指定しています。

## 構文

```css
プロパティ名: 値;
```

の形でスタイルを指定します。

```css
color: red;
font-size: 20px;
```

このように指定した場合、HTML 要素は、

- 文字の色（`color`） が、赤色（`red`）
- 文字のサイズ（`font-size`）が、`20px`

になります。

## 使用されるプロパティの例

- `color`: テキストの色を指定
- `font-size`: テキストのサイズを指定
- `background-color`: 背景色を指定

他にも指定できるプロパティは数多くあります。
詳しくは、[Appendix 1. プロパティについて詳しく](./a1_style_properties.md) を見てください。

### [補足説明]カラーコードについて

色の指定は、色の名前で行う他に、カラーコード（`#ffffff`、`#414bb2`）、rgb 値（`rgb(224, 224, 244)`）で行うことができます。

カラーコード、rgb については、

- [<hex-color> - 開発者向けのウェブ技術 | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/hex-color)
- [<color> - 開発者向けのウェブ技術 | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/color_value)

を参照してください。

## 実践

早速使ってみましょう。
前回作成した、HTML ファイルに追記していきます。

`h1` 要素に style 属性を追加し、

- 文字色を白
- 背景色を赤
- 文字のサイズを 30px

に指定します。

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>[ここにあなたのGitHubユーザー名を入力]</title>
  </head>
  <body>
    <h1 style="color: white; background-color: red; font-size: 48px;">
      [ここにあなたのGitHubユーザー名を入力]'s page
    </h1>
  </body>
</html>
```

追加し、プレビューするとこのようになると思います。

![見出し1が装飾される](./images/style-attribute-1.png)

このように表示されたら成功です！

## 練習問題

それでは練習問題をやってみましょう。

Q. 以下のうち、正しい style 属性の書き方はどれでしょうか？

<hr>

A.

```html
<p style="color: blue font-size: 16px;">からあげ</p>
```

B.

```html
<div style="background-color=yellow; color=blue;">ハンバーグ</div>
```

C.

```html
<span style="color: red; font-size: 32px;">とんかつ</span>
```

D.

```html
<h1 style="font-size: 24px: background-color: green;">肉を甘辛く炒めたやつ</h1>
```

<hr>
<br>

<details>
  <summary>A. が解答だと思ったらクリック</summary>
   間違いです。プロパティを区切るセミコロン（;）がありません。
</details>
<br>

<details>
  <summary>B. が解答だと思ったらクリック</summary>
   =を使ってプロパティと値を結びつけているため、間違いです。正しくはコロン（:）を使います。
</details>
<br>

<details>
  <summary>C. が解答だと思ったらクリック</summary>
   正解です！とんかつ、美味しいですよね（？）
</details>
<br>

<details>
  <summary>D. が解答だと思ったらクリック</summary>
   コロン（:）を使ってプロパティを区切っているため、間違いです。正しくはセミコロン（;）を使います。
</details>
<br>

<br>
では次に進みましょう。
