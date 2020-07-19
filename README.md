# HSP3-constant

**ダウンロード(リリース)は右部のreleasesか[こちら](https://github.com/UMAGODi/HSP3-constant/releases)**

## 概要

### 概要・使用法 [constant.as]

青い葉っぱさん(http://hp.vector.co.jp/authors/VA034288/) が公開している「WIN32API定数」をベースにHSP3でインクルードして使用できるように編集したものです。  
commonフォルダーにコピーしてスクリプトの先頭に「#include "constant.as"」を記述することでHSP3でWin32API 定数を使用することができます。<br>
(constant.asをインクルードすればconstant_p1.as ～ constant_p7.as が自動的にインクルードされるので、それらを個別にインクルードする必要はありません。)



HSP3は未使用定義をコンパイル時に自動的に除去する機能があるので、**インクルードしてもファイルサイズが特別大きくなる
ことはありません。**

全ての定数を検証したわけではないので、一部 値が間違っている可能性があります。もしお気づきの場合はissueにでも報告していただけると助かります。



内容が多いためソートして7パートに分割しました。

constant.as：以下7つをインクルード<br>
constant_p1.as：A～C<br>
constant_p2.as：D～E<br>
constant_p3.as：F～I<br>
constant_p4.as：J～M<br>
constant_p5.as：N～P<br>
constant_p6.as：Q～S<br>
constant_p7.as：T～_




### 概要・使用法 [constant.hs]

上記のconstant.asで定義されている定数をHSPドキュメントライブラリ(以下 HDL)で検索できるようにしたドキュメントファイルです。  

constant.hs を `(HSPフォルダー)/doclib` または `(HSPフォルダー)/hsphelp` にコピーした後にHDLを起動すると読み込まれます。  
すでにHDLを実行している場合はHDLを再起動してください。  
導入後 HDL初回起動時の読み込みに少し時間がかかる場合があります。

**HSP 3.6beta未満のHDLでは正しく表示できないという情報をいただきました。もしHSP 3.6beta未満の環境の方で正しく表示できない方はHSPのアップグレードをしてみてください。**



内容が多いためソートして7パートに分割しました。

constant_p1.hs：A～C<br>
constant_p2.hs：D～E<br>
constant_p3.hs：F～I<br>
constant_p4.hs：J～M<br>
constant_p5.hs：N～P<br>
constant_p6.hs：Q～S<br>
constant_p7.hs：T～_



## Ver. 1.2.0における新規導入、アップグレード方法

### 【新規に導入する場合】

基本的には上記の概要と手順は同じです。

commonフォルダー及びhsphelpフォルダーを自分が使ってるHSPのルートフォルダ(hsed.exeやhsp3.exe等があるフォルダ)にコピーまたは移動してください。<br>もしくは同梱のファイルをそれぞれのフォルダーと同じ名前のフォルダー(common、hsphelp)の中にコピーまたは移動してください。

### 【過去のバージョンの constant.as 及び constant.hs からアップグレードする場合】

* common/constant.as　→　上書き
* hsphelp/constant.hs　→　**削除**
* その他新規ファイル　→　コピーまたは移動



## 変更履歴

### マイナーアップデート [2020/07/19]
**マイナーアップデートではリリースは更新されません。マイナーアップデートはレポジトリ内のファイルの更新のみ行われます。**<br>
**マイナーアップデートの内容は次のバージョンのリリース時にまとめて追加されます。**

* LB_DELETESTRING, LB_FINDSTRINGEXACT, LB_GETLISTBOXINFO, LB_GETSELCOUNT, LB_GETSELITEMS, LB_GETTEXTLEN, LB_MULTIPLEADDSTRING, LBS_NOTIFY, LBS_OWNERDRAWFIXED, LBS_OWNERDRAWVARIABLE, LBS_COMBOBOX を追加。`constant.as` `constant.hs`
* LBS_STANDARD の定義を更新。(展開後の値は変化していません) `constant.as` `constant.hs`

### v1.2.0 [2020/07/15]

* #funcの引数と干渉するためNULLPTRを削除 (配慮が足りていませんでした。申し訳ありません。) `constant.as` `constant.hs`
* 内容をソートし7つのパートに分割 `constant.as` `constant.hs`

### v1.1.2 [2020/03/16]

* WS_MAXIMIZEBOXを追加 `constant.as` `constant.hs`

### v1.1.1 [2020/03/05]

* NULLPTRを追加 ($00000000 で定義) `constant.as` `constant.hs`

### v1.1.0 [2020/02/10]
* 定数検索アプリを廃止しHSPドキュメントライブラリ用の constant.hs を作成 `constant.hs`
* 書式等細かい調整 `constant.as`
* 「LVM_FIRST」が「  FIRST」になっていた問題を修正 `constant.as`
* いくつかの足りていなかった定数を追加 `constant.as`

### v1.0.1 [2018/10/25]
* 初版
* github未公開
