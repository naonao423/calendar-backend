# calender-backend

## ホームページのグラフを表示するためのカレンダーの内容読み取りプログラム。
本プログラムは Chalice AWSで作られています。

## プログラムの流れ
### 前提条件
まずiphoneのshortcutで勉強した内容を公にしていいcalendarに記録させます。
次にそのカレンダーをpublicにして外部からurlでicsのファイルをダウンロードできるようにします。

### 本プログラム
そのurlからダウンロードしたicsを取り込んで自分のほしいようなdataに作り替えるプログラムを作成(parse)
→/vender/internalpackage/botocal.py
それを読み込みdynamoDBの保存する関数を作成。
→/chalicelib/database.py 内のreload関数

## それ以外に
ホームページのグラフ表示に適したような関数がdatabase.pyに格納されている。

