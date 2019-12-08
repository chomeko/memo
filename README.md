# chomekoメモ
- 文章のフォントサイズ
>近年のwebページは行の高さを大きくとり<br>
>文章全体をゆったりと大きくする傾向がある。<br>
>line-heightで行の高さを１.８倍にしてる<br>
>行の高さ = font-size14pxの１.８倍 = 25.2px

# 便利ツール
- Adobe Color cc 配色サイト
- gogle fonts フォントサイト
- https://fontawesome.com/ アイコンフォトサイト

# vwの計算
- １vwは画面横幅の100分の1になる
>例)<br>
>画面横幅が３２０pxの時にh１要素を４８pxで表示したい時<br>
>1vw = 3.2px<br>
>48 % 3.2 = 15 になるから<br>
>48px = 15vw

# emの計算
- フォントサイズ = 1em
>例）<br>
>font-sizeが115pxだとすると<br>
>1em = 115px<br>
>0.1em = 11.5px<br>
>0.2em = 23pxとなる

## === gulpコマンド集 ===
- npx gulp タスクランナー
- gulp imagemin 画像圧縮
## === emmet-html コマンド集 ===
- html:5 雛形
- link:css 読み込むcss設定
- sec セクション
- . div class=""
- section.  section class=""
- ul>li*5>a[href=#]
```
ul
  li
    a(href="#")
  li
    a(href="#")
  li
    a(href="#")
```
### === sass(css) メモ集 ===
- div:not(:first-child)
>first-childで親要素内の１つ目の子要素が適用される
>子要素はこの場合divになる
>notをつけることで１つ目以外の子要素に適用される
- 親 display: flex
>各子要素にflex:1で等倍
- flex-wrap: wrap
>横に並べたパーツの横幅が１００％を超えたら
>カラム落ちで下に表示さす
>各子要素に％を指定
```
footer
  .container
    display: flex
    flex-wrap: wrap
.footA
  flex: 0 0 40%
.footB
  flex: 0 0 60%
  display: flex
  div
    flex: 1
.footC
  flex: 100%
```
- 円
>emでフォントサイズの２倍
>中央の50%
```
width: 2em
line-height: 2em
border-radius: 50%
```
## === emmet-sass コマンド集 ===
- c# `color: #カラーコード`
- c:i `color: inherit`
- bc `background-color:`
- mt `margin-tpo`
- mb `margin-bottom`
- m0-a `margin: 0 auto`
- ml:a `margin-left: auto`
- mr:a `margin-right: auto`
- fz `font-size`
- w `width:`
- h `height:`
- lh `line-height`
- op `opacity`
- ll `list-style`
- tdn `text-decoration: none`
- tdu `text-decoration: underline`
- ta:c `text-align: center`
- dib `display: inline-block`
- df `display: flex`
- fxd:rr `flex-direction: row-reverse`
- fx:1 `flex:1`
- bdrs `border-radius:`
- mnw `min-width:`
- mxw `max-width:`
## === pug  ===
- a(href="#") 文字
- p 文字の改行
```
p 〒000-0000  東京都中央区杉並3-3-403
  br
  a(href="#") http://logger.nett/
```
- 代替テキストを非表示設定
```
span.fa.fa-twitter(title="Twitter",aria-hidden="true")
  span.sr-only Twitter

```
```
style(type='text/css').
  .sr-only {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect( 0,0,0,0 );
    border: 0;
  }
```
