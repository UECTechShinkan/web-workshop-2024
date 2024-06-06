# 4-4. 実際に WEB サイトを作ろう（3/3）

## `main`のスタイル

```html
<main>
  <img
    src="./images/header-image.png"
    alt="大学院オープンラボ2024"
    class="top-banner"
  />
  <section id="uec-research">
    <h2>UEC Research</h2>
    <ul class="card-list">
      <li>
        <h4>
          「光と原子の新たな量子技術」電気通信大学Ⅲ類（理工系）丹治はるか准教授
        </h4>
        <p>
          最前線の量子研究、光の研究について、丹治はるか准教授（Ⅲ類（理工系）、基盤理工学専攻）と学生さんが紹介します。
        </p>
      </li>
      <li>
        <h4>「ヘビ型ロボットの開発」電気通信大学Ⅱ類（融合系）田中基康教授</h4>
        <p>
          最前線のロボット研究について、田中基康教授（Ⅱ類（融合系）、機械知能システム学専攻）と学生さんが紹介します。
        </p>
      </li>
      <li>
        <h4>
          「人とコンピュータが融合する社会」電気通信大学Ⅰ類（情報系）橋本直己教授
        </h4>
        <p>
          最前線の仮想現実（バーチャルリアリティ）研究について、橋本直己教授（Ⅰ類（情報系）、情報学専攻）と学生さんが紹介します。
        </p>
      </li>
      <li>
        <h4>UEC Research & Innovation</h4>
        <p>
          The January 2024 issue of UEC Research and Innovationincludes video
          profiles of UEC faculty Katsuya Suto...
        </p>
      </li>
    </ul>
  </section>
  <section id="news">
    <h2>重要なお知らせ</h2>
    <ul class="news-list">
      <li>
        令和６年能登半島地震で被災された方へのお見舞い（田野学長メッセージ）
      </li>
      <li>《在学生対象》令和６年能登半島地震への対応について</li>
      <li>令和６年度新入生のみなさまへ</li>
    </ul>
  </section>
</main>
```

---

見出し 2（`h2`）に関する設定です。

`text-align: center;`でテキストを中央揃えしています。

```css
h2 {
  font-size: 2rem;
  text-align: center;

  color: #17288b;
}
```

---

トップバーナー（画像）に関する設定です。
画像の幅を画面と同じにすることではみ出しを防いでいます。

```css
.top-banner {
  display: block;

  width: 100%;
}
```

---

グリッドを用いてグリッドアイテムを 4 つ並べるように設定しています。
また、`gap: 1rem;`でアイテム間の空白を`1rem`に設定しています。

```css
.card-list {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;

  width: 100%;

  padding: 1rem;

  gap: 1rem;

  list-style-type: none;
}

.card-list li {
  padding: 1rem;

  border: 1px solid #ccc;
}

.card-list li h4 {
  font-size: 1rem;
}

.card-list li p {
  font-size: 0.8rem;
}
```

---

それぞれのお知らせについて、高さを固定し、flexbox を用いて文字を置く場所を調節しています。

また、`:first-child`などを用いることで、「何番目の要素にだけこのスタイルを適応する」という指定をしています。

```css
.news-list {
  list-style-type: none;

  margin: 1rem;
}

.news-list li {
  display: flex;
  align-items: center;

  justify-content: center;

  width: 100%;
  height: 4rem;

  padding: 0 1rem;

  color: #ffffff;

  font-weight: bold;
}

.news-list li:first-child {
  background-color: #e8e803;
  color: #888888;
}

.news-list li:nth-child(2) {
  background-color: #e65100;
}

.news-list li:last-child {
  background-color: #25b7c0;
}
```

## 完成

ここまで、すべてのスタイルが設定できたら、完成です！

...が、まだまだ、改善点はたくさんあります。
余裕がありそうな人は、是非発展課題にチャレンジしてみてください！

### 発展課題（解答は余力があれば作るかも？）

- ヘッダーの「電気通信大学」を実際に使用されている画像に変えてみましょう
- ヘッダーのメニューが狭い画面幅で表示したときに崩れてしまうので、前回やったメディアクエリを使って改善してみましょう
- UEC Research のカードに画像を埋め込んでみましょう
- UEC Research もヘッダーと同様、狭い画面幅で表示した場合に崩れてしまうので、対処を考えて見ましょう
- 重要なお知らせをマウスでホバーしたときのアニメーションをつけてみましょう（[大学 HP](https://www.uec.ac.jp/)参照）
- フッターの SNS をロゴで表示してみましょう

などなど、他にもなにか思いついた機能があれば、自分で実装してみると実力が確実に上がります。
わからないことがあれば、これまでの講習の講師や Google 先生など有識者に、聞いてみることが重要です！
