
# HTMLとMarkdownの対応表

| HTMLタグ           | Markdown形式   | 意味                      | MDNリンク                                                |
|--------------------|----------------|---------------------------|---------------------------------------------------------|
| `<h1>`             | `#`            | 見出し1                   | [MDN h1](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |
| `<h2>`             | `##`           | 見出し2                   | [MDN h2](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |
| `<h3>`             | `###`          | 見出し3                   | [MDN h3](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |
| `<h4>`             | `####`         | 見出し4                   | [MDN h4](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |
| `<h5>`             | `#####`        | 見出し5                   | [MDN h5](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |
| `<h6>`             | `######`       | 見出し6                   | [MDN h6](https://developer.mozilla.org/ja/docs/Web/HTML/Element/Heading_Elements) |
| `<p>`              | *段落の開始(前の行との間に1行以上の改行を入れる)*   | 段落                      | [MDN p](https://developer.mozilla.org/ja/docs/Web/HTML/Element/p) |
| `<strong>`         | `**` or `__`   | 強調                      | [MDN strong](https://developer.mozilla.org/ja/docs/Web/HTML/Element/strong) |
| `<em>`             | `*` or `_`     | 斜体                      | [MDN em](https://developer.mozilla.org/ja/docs/Web/HTML/Element/em) |
| `<a href="url">text</a>`              | `[text](url)`  | ハイパーリンク            | [MDN a](https://developer.mozilla.org/ja/docs/Web/HTML/Element/a) |
| `<img alt="alt" src="url">`            | `![alt](url)`  | 画像                      | [MDN img](https://developer.mozilla.org/ja/docs/Web/HTML/Element/img) |
| `<ul>`             | `*`または`-`   | 箇条書きリスト            | [MDN ul](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ul) |
| `<ol>`             | `1.`           | 番号付きリスト            | [MDN ol](https://developer.mozilla.org/ja/docs/Web/HTML/Element/ol) |
| `<li>`             | *リスト項目*   | リストの項目              | [MDN li](https://developer.mozilla.org/ja/docs/Web/HTML/Element/li) |
| `<blockquote>`     | `>`            | 引用                      | [MDN blockquote](https://developer.mozilla.org/ja/docs/Web/HTML/Element/blockquote) |
| `<hr>`             | `---`          | 水平線                    | [MDN hr](https://developer.mozilla.org/ja/docs/Web/HTML/Element/hr) |
| `<br>`             | `` (2 spaces)| 改行                      | [MDN br](https://developer.mozilla.org/ja/docs/Web/HTML/Element/br) |

## `<a>`要素と`<img>`要素に関する補足

### `<a>`要素

以下の2つは同じ意味になります。

```html
<a href="https://example.com">example</a>
```

```markdown
[example](https://example.com)
```

### `<img>`要素

以下の2つは同じ意味になります。

```html
<img alt="alt" src="https://upload.wikimedia.org/wikipedia/commons/7/70/Example.png">
```

```markdown
![alt](https://upload.wikimedia.org/wikipedia/commons/7/70/Example.png)
```
