# プロパティについて詳しく

使用できるプロパティのうち、よく使われるものです。
他にも詳しく見たい場合は、

- [CSS リファレンス - CSS: カスケーディングスタイルシート | MDN](https://developer.mozilla.org/ja/docs/Web/CSS/Reference#%E7%B4%A2%E5%BC%95)

あたりを見るか、「CSS プロパティ一覧」などで検索すると良いと思います。

| プロパティ                                                                                | 説明                                                 | 例                                    |
| ----------------------------------------------------------------------------------------- | ---------------------------------------------------- | ------------------------------------- |
| [`color`](https://developer.mozilla.org/en-US/docs/Web/CSS/color)                         | テキストの色を指定します。                           | `color: red;`                         |
| [`background-color`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-color)   | 要素の背景色を指定します。                           | `background-color: yellow;`           |
| [`font-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-size)                 | フォントサイズを指定します。                         | `font-size: 16px;`                    |
| [`font-weight`](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight)             | フォントの太さを指定します。                         | `font-weight: bold;`                  |
| [`text-align`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-align)               | テキストの揃え方を指定します。                       | `text-align: center;`                 |
| [`margin`](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)                       | 要素の外側の余白を指定します。                       | `margin: 10px;`                       |
| [`padding`](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)                     | 要素の内側の余白を指定します。                       | `padding: 10px;`                      |
| [`border`](https://developer.mozilla.org/en-US/docs/Web/CSS/border)                       | 要素の枠線を指定します。                             | `border: 1px solid black;`            |
| [`width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width)                         | 要素の幅を指定します。                               | `width: 100px;`                       |
| [`height`](https://developer.mozilla.org/en-US/docs/Web/CSS/height)                       | 要素の高さを指定します。                             | `height: 50px;`                       |
| [`display`](https://developer.mozilla.org/en-US/docs/Web/CSS/display)                     | 要素の表示形式を指定します。                         | `display: block;`                     |
| [`position`](https://developer.mozilla.org/en-US/docs/Web/CSS/position)                   | 要素の位置指定方法を設定します。                     | `position: absolute;`                 |
| [`top`](https://developer.mozilla.org/en-US/docs/Web/CSS/top)                             | 上からの位置を指定します。                           | `top: 10px;`                          |
| [`left`](https://developer.mozilla.org/en-US/docs/Web/CSS/left)                           | 左からの位置を指定します。                           | `left: 20px;`                         |
| [`right`](https://developer.mozilla.org/en-US/docs/Web/CSS/right)                         | 右からの位置を指定します。                           | `right: 30px;`                        |
| [`bottom`](https://developer.mozilla.org/en-US/docs/Web/CSS/bottom)                       | 下からの位置を指定します。                           | `bottom: 40px;`                       |
| [`float`](https://developer.mozilla.org/en-US/docs/Web/CSS/float)                         | 要素を左右に浮かべて配置します。                     | `float: left;`                        |
| [`clear`](https://developer.mozilla.org/en-US/docs/Web/CSS/clear)                         | `float`を解除する位置を指定します。                  | `clear: both;`                        |
| [`z-index`](https://developer.mozilla.org/en-US/docs/Web/CSS/z-index)                     | 要素の重なり順序を指定します。                       | `z-index: 10;`                        |
| [`overflow`](https://developer.mozilla.org/en-US/docs/Web/CSS/overflow)                   | 要素内の内容が溢れたときの処理を指定します。         | `overflow: hidden;`                   |
| [`visibility`](https://developer.mozilla.org/en-US/docs/Web/CSS/visibility)               | 要素の表示・非表示を指定します。                     | `visibility: hidden;`                 |
| [`opacity`](https://developer.mozilla.org/en-US/docs/Web/CSS/opacity)                     | 要素の不透明度を指定します。                         | `opacity: 0.5;`                       |
| [`border-radius`](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius)         | 要素の角を丸くする半径を指定します。                 | `border-radius: 5px;`                 |
| [`box-shadow`](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)               | 要素に影をつけます。                                 | `box-shadow: 2px 2px 5px gray;`       |
| [`text-shadow`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow)             | テキストに影をつけます。                             | `text-shadow: 1px 1px 2px black;`     |
| [`background-image`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-image)   | 背景画像を指定します。                               | `background-image: url('image.jpg');` |
| [`background-size`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-size)     | 背景画像のサイズを指定します。                       | `background-size: cover;`             |
| [`background-repeat`](https://developer.mozilla.org/en-US/docs/Web/CSS/background-repeat) | 背景画像の繰り返し方法を指定します。                 | `background-repeat: no-repeat;`       |
| [`line-height`](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height)             | 行間の高さを指定します。                             | `line-height: 1.5;`                   |
| [`letter-spacing`](https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing)       | 文字の間隔を指定します。                             | `letter-spacing: 1px;`                |
| [`text-transform`](https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform)       | テキストの大文字・小文字変換を指定します。           | `text-transform: uppercase;`          |
| [`white-space`](https://developer.mozilla.org/en-US/docs/Web/CSS/white-space)             | 空白文字の処理方法を指定します。                     | `white-space: nowrap;`                |
| [`cursor`](https://developer.mozilla.org/en-US/docs/Web/CSS/cursor)                       | マウスポインターの形状を指定します。                 | `cursor: pointer;`                    |
| [`transition`](https://developer.mozilla.org/en-US/docs/Web/CSS/transition)               | CSS プロパティの変化にアニメーションを適用します。   | `transition: all 0.3s ease;`          |
| [`transform`](https://developer.mozilla.org/en-US/docs/Web/CSS/transform)                 | 要素を変形します（回転、拡大縮小、移動、傾斜など）。 | `transform: rotate(45deg);`           |
| [`animation`](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)                 | 要素にアニメーションを適用します。                   | `animation: myAnimation 2s infinite;` |
| [`content`](https://developer.mozilla.org/en-US/docs/Web/CSS/content)                     | 擬似要素にコンテンツを挿入します。                   | `content: 'Hello';`                   |
