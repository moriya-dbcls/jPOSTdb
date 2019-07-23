# [https://tinyurl.com/2019-jpost](https://tinyurl.com/2019-jpost)にアクセスすると、このページが開きます

# JPrOS 2019 jPOSTショートコース <br>- jPOSTdbで公開されているデータの見方 -
情報・システム研究機構
データサイエンス共同利用基盤施設
ライフサイエンス統合データベースセンター  
守屋 勇樹 moriya@dbcls.rois.ac.jp  
2019/07/27 宮崎 

--
## 講習会の流れ  

今回のショートコースでは、ウェブブラウザを使って jPOSTdb の操作を行います
  - jPOSTdbの概要
  - データセットを検索してみる
    - データセットページの概要
  - タンパク質を検索してみる
   - タンパク質ページの概要
  - Sliceとは？
  - Sliceを作成してみる
  - ２つのSliceを比較してみる

--
#### 講習に際しての注意とお願い

- みんなで同時にアクセスするとサイトにつながりにくくなることが予想されます。
  - 資料を見ながら自力で進められそうな方はどんどん先に、そうでない方は一緒にすすめていきましょう。
  - サイトの反応が悪い時はタイミングをずらして実行してみてください。
  - 反応が無いからと言って何度もクリックするとますます繋がらなくなってしまいます。おおらかな気持ちで臨みましょう。
- わからないことがあったら挙手にてスタッフにお知らせください。
  - 遠慮は無用です(そのための講習会です!)。おいてけぼりは楽しくありません。
- 今回のコースでは一応Google Chromeを推奨いたしますが、Firefox、Safari、Edge、Operaなどのモダンブラウザでも問題ないと思います。ただしInternet Explorerは古すぎるので動作を保証していません。モバイル機器でのタッチパネル操作も一部未対応です。
---
## jPOSTdbとは
jPOSTdbは質量分析に基づくプロテオームデータを"再解析"をし、その結果を収録したデータベースです。

![jpost](https://github.com/moriya-dbcls/jPOSTdb/blob/master/2019/images/jpost.png)

repositoryに登録したデータを直接見れるわけではありません。

- 収録されたデータセット毎にプロテオームデータを俯瞰できます
  - Protein EvidenceやKEGG Pathwayへのマッピングができます
- タンパク質毎に同定されたペプチドやisoformの情報を見ることができます
- 興味のあるデータセット複数を切り出して、データを俯瞰できます（Slice）
- 簡易的なツールを用いてSlice間の比較を行うことができます

---
## [jPOSTdb webサイト](https://globe.jpostdb.org/)

![jpost](https://github.com/moriya-dbcls/jPOSTdb/blob/master/2019/images/jpostdb_01.png)

- Topページ
  - 最初に、データベースに入っているデータセットの生物種の割合を示したチャートが出ます
    - マウスカーソルをホバーさせることで、詳細が表示されます
  - 下にはデータセットのリストテーブルが表示されます
    - 2019/7/27時点で103データセットが収録されています
    - "DS59_1" というのがjPOSTdbでのデータセットのIDになっています
  - 上のpie chartのある部分はデータセットの絞り込みを行うフォームになっています

---
## データセットを絞り込んでみよう
- 例えばhumanで絞りこみをしてみましょう
  - テキストエリアをクリックすると候補が表示されます。クリックで選択されます
  - pie chartをクリックすることでも選択できます

![jpost](https://github.com/moriya-dbcls/jPOSTdb/blob/master/2019/images/jpostdb_02.png)

- テーブルのリストが66データセット、14,620タンパク質に減りました
- 生物種以外に、Sample type、Cell line、Organ、Disease、Mofdification、Instrumentで絞り込みが行なえます
- "+" ボタンをクリックすることで、複数のカテゴリで絞り込みを行うことができます

---
## データセットを検索絞してみよう
- 一旦全部の絞り込みを外しましょう
- テーブルの上にワード検索Boxがあります。キーワードに関連したデータセットが検索されます
  - データがまだ少ないので、今回は"fibroblast"で検索

![jpost](https://github.com/moriya-dbcls/jPOSTdb/blob/master/2019/images/jpostdb_03.png)

- 9つのデータセットが引っかかり、5,711タンパク質が収録されていました

---
## データセットの中身を見ていこう
- テーブルの "DS87_1" をクリックしてデータセットDS87_1の中身を表示しましょう

![jpost](https://github.com/moriya-dbcls/jPOSTdb/blob/master/2019/images/jpostdb_04.png)
