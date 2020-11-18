## タグの種類
- h1,h2... :heading 見出しのこと
- p :paragraph 段落
- a :リンク,hrefにurlを入力可能,インライン要素に注意(幅と高さとmarginの設定不可)
- img :srcに画像のurlを入力
- li :リスト,ulで囲むと黒点,olで囲むと数字
- div :division,要素をグループ化する際に使用
- inputとtextarea:1行か複数行入力可能かの違い,inputはtype="submit"で送信可能,value=""で好きなテキストに
## htmlの構造
```
<html>
    <head>
    </head>
    <body>
    </body>
</html>
```

### headの要素
```
<title></title>でページタイトル作成
<link rel="stylesheet" href="名前.css">でcssファイルを読み込み可能
```
### bodyの要素
基本的にwebサイトはヘッダー、メイン、フッターの３つで構成されることが多い


## css
- 横並びにする方法:floatでrightやleftを指定し横並びになる
- 余白の調整:paddingとmargin,paddingはborderの内側,marginは外側
- 枠線:  border:太さ 種類 色;
- 背景に画像:  background-image:url(~~~); ただし画像のサイズの調整が必要な場合が多い,調整は基本background-size:cover;
- 中央寄せ: marginの左右を"auto"にする
- 文字の透明感: opacityで決める、0~1で
- 背景のみ透明に: rgbaを使う、rgba(①,②,③,④)と入力し④で透明度を設定する
- 文字の間隔:letter-spacing
- インラインとブロックとインラインブロック:displayプロパティで変更可能
- カーソルが乗ったときの状態の操作:  ":hover"をclassの右につける
- 角の丸み:border-radius
- テキストの要素の配置の指定: text-alignプロパティ　left,conter,rightで
- アニメーションをつける:　"translation:all time;"を使う、allは変化の対象のことでありこう指定するとすべてのプロパティに適用できる、timeは変化する時間
- 行の高さ:line-height,要素を縦方向の中央に揃えることも可
- 文字の太さ: font-weight
- 相対的なサイズ:weightやheightを%で指定する
- 要素を重ねる: "position:absolute;"を指定した要素は重ねられる様になる、この場合基準点からどれくらい移動させるかを決める
- 基準位置:"position:relative;"を指定した要素の左上部分が基準になる
- ボックスの立体感: "box-shadow:水平方向 垂直方向 色;"
- カーソル: coursorで変更可能
- クリックされている間の動き: ":active"をクラスの右につける
- 画面に要素を固定: "position:fixed;"位置は"top,left,right,bottom"で指定
- 重なりの順序:z-indexを指定し値が大きいほど上に表示
## その他
- 一部の文にCSSを適用:spanで囲む
- 複数のクラス名の設定:"a b"のようにスペースを入れると可能、どちらでも呼び出せる
- コメントの挿入: htmlは ```<!--  -->```     cssは/*  */

## Font Awesomeの使い方
1. 読み込むために```<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css">```
2. spanタグに"fa fa-アイコン名"のクラスを指定
