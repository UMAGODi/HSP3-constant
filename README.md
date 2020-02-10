# HSP3-constant

**ダウンロード(リリース)は上部のreleasesか[こちら](https://github.com/UMAGODi/HSP3-constant/releases)**

### 概要・使用法 [constant.as]

青い葉っぱさん(http://hp.vector.co.jp/authors/VA034288/) が公開している「WIN32API定数」をベースにHSP3でインクルードして使用できるように編集したものです。  
commonフォルダーにコピーしてスクリプトの先頭に「#include "constant.as"」を記述することでHSP3でWin32API 定数を
使用することができます。

HSP3は未使用定義をコンパイル時に自動的に除去する機能があるので、**インクルードしてもファイルサイズが特別大きくなる
ことはありません。**

全ての定数を検証したわけではないので、一部 値が間違っている可能性があります。


### 概要・使用法 [constant.hs]

上記のconstant.asで定義されている定数をHSPドキュメントライブラリ(以下 HDL)で検索できるようにしたドキュメントファイルです。  

constant.hs を `(HSPフォルダー)/doclib` または `(HSPフォルダー)/hsphelp` にコピーした後にHDLを起動すると読み込まれます。  
すでにHDLを実行している場合はHDLを再起動してください。  
導入後 HDL初回起動時の読み込みに少し時間がかかる場合があります。
