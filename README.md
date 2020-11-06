# dataAndDung
古典的三次元ダンジョンのデータの持ち方

```
//virtual key
A=fn_keyA
B=fn_keyB
X=fn_keyX
Y=fn_keyY
L=fn_keyL
R=fn_keyR
<=fn_arrowL
>=fn_arrowR
^=fn_arrowU
v=fn_arrowD
//symbolの一括設定
wall=壁■□
door=扉
doorkey=鍵ＡＢＣＤＥＦＧＨＩＪＫＬＭＮＯＰＱＲＳＴＵＶＷＸＹＺ
doorsec=隠
//door系統はAボタンで開ける。
road=　街毒闇痺宝↑↓←→ //十字キーで移動可能 wall door系以外は全て移動可能で設定する意味は無く、メモ程度。
//
sあ=aaaa.png,16,9 //立ち絵のイメージ。そのシンボルに乗った時の立ち絵。
tあ=これは｜テキスト｜改行は縦ハイフン
qあ=この象は何の像だろうか？｜馬｜猿｜羊｜＊いや象 //＊は正答。正答の場合、FLG('あ')にフラグ、1が立つ
fあ=fn_aa //function call そのシンボルに乗った瞬間に呼ばれる。特殊な場合のみ。
//t q fの順に呼ばれるが、ひとつに設定する事を推奨
あ=wall //シンボルのタイプ。壁か扉か鍵か隠か道 wall door doorkey doorsec road
gあ=#0f0 //地面の色、指定しない場合は壁の色。毒などの区別。
iあ=！ //アイコン表示。文字のみ。アイコン表示が必要な場合のみ設定する。ここでは！
mあ=！ //ミニマップ上のシンボル、壁は色のみの設定。
//mapdata
fF00=fn_F00 //その層にいる時、キーイベントの前の呼ばれる。例えばランダムエンカウントや情報表示。
wF00=xxxxyyyy.jpg
F00.
//mapdata string
END

```
