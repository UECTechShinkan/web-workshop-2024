# 様々なセレクタの指定方法

> [!WARNING]
> 時間がなかったので、ChatGPT に書かせました。
> ぱっと見た感じ、特に間違いはなさそうですが、ちゃんと知りたい人は自分で調べながら読むことをおすすめします。
>
> ところで ChatGPT 4 に課金しようかと思っていたりします、すごいらしいですねあの子

CSS では、子要素や孫要素などの特定の要素を選択するためのセレクタがあります。これにより、階層構造に基づいてスタイルを適用できます。主なセレクタとして、子要素セレクタ、子孫セレクタ、隣接兄弟セレクタ、一般兄弟セレクタがあります。以下、それぞれのセレクタについて詳しく説明します。

## 子要素セレクタ ( `>` )

子要素セレクタは、ある要素の直下にある特定の要素を選択します。

HTML:

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>子要素セレクタの例</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="container">
      <p>これは通常の段落です。</p>
      <p>これも通常の段落です。</p>
      <div>
        <p>これはネストされた段落です。</p>
      </div>
    </div>
  </body>
</html>
```

CSS (`styles.css`):

```css
.container > p {
  color: blue;
}
```

この例では、`.container` の直下にある `<p>` 要素だけが青色になります。ネストされた `<p>` 要素には適用されません。

## 子孫セレクタ (スペース)

子孫セレクタは、ある要素のすべての子孫要素を選択します。これには子要素、孫要素、さらにその下の要素も含まれます。

HTML:

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>子孫セレクタの例</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="container">
      <p>これは通常の段落です。</p>
      <p>これも通常の段落です。</p>
      <div>
        <p>これはネストされた段落です。</p>
      </div>
    </div>
  </body>
</html>
```

CSS (styles.css):

```css
.container p {
  color: green;
}
```

この例では、`.container` のすべての`<p>`要素（子要素と孫要素の両方）が緑色になります。

## 隣接兄弟セレクタ ( `+` )

隣接兄弟セレクタは、ある要素の直後に続く兄弟要素を選択します。

HTML:

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>隣接兄弟セレクタの例</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>見出し1</h1>
    <p>これは段落です。</p>
    <h1>見出し2</h1>
    <p>これは別の段落です。</p>
  </body>
</html>
```

CSS (styles.css):

```css
h1 + p {
  color: red;
}
```

この例では、`<h1>`要素の直後にある`<p>`要素が赤色になります。

## 一般兄弟セレクタ ( `~` )

一般兄弟セレクタは、ある要素の後に続くすべての兄弟要素を選択します。

HTML:

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>一般兄弟セレクタの例</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>見出し1</h1>
    <p>これは段落です。</p>
    <p>これも段落です。</p>
    <h1>見出し2</h1>
    <p>これは別の段落です。</p>
  </body>
</html>
```

CSS (styles.css):

```css
h1 ~ p {
  color: purple;
}
```

この例では、`<h1>`要素の後に続くすべての`<p>`要素が紫色になります。

## 具体的な利用例

これらのセレクタを組み合わせることで、より複雑なスタイル適用が可能になります。

HTML:

```html
<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>セレクタの組み合わせ例</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="container">
      <p>これは通常の段落です。</p>
      <p>これも通常の段落です。</p>
      <div>
        <p>これはネストされた段落です。</p>
        <span>これはネストされたスパン要素です。</span>
      </div>
      <span>これは兄弟スパン要素です。</span>
    </div>
  </body>
</html>
```

CSS (styles.css):

```css
.container > p {
  color: blue;
}

.container p {
  font-weight: bold;
}

.container > div > p {
  color: green;
}

.container span {
  color: red;
}
```

この例では、複数のセレクタを組み合わせて、異なる階層にある要素に対して異なるスタイルを適用しています。

- `.container > p` は、.container の直下にある`<p>`要素を青色にします。
- `.container p` は、.container 内のすべての`<p>`要素を太字にします。
- `.container > div > p` は、.container の直下の`<div>`内の`<p>`要素を緑色にします。
- `.container span` は、.container 内のすべての`<span>`要素を赤色にします。

これにより、階層構造に基づいて詳細なスタイル指定が可能になります。
