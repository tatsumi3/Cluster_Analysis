statistical_clistering_method
======================
概要は省略

sorting_packetフォルダにはファイル読み込みをするためパケット数を操作するプログラムになっている。
 
使い方
------
### main.rb ###
読み込むファイルを指定する必要があります。このプログラムのためのファイルの生成は後のsorting_packetフォルダで行います。
また、実行後にdev_【ファイル名】.txtとR_k_【ファイル名】.txtというtxtファイルが生成されます。使用方法は以下の通りです。

	$ ruby main.rb 【ファイル名】
 (注)Rubyは1.9.3以降を使用する必要があります。

### sorting_packet/read_in_packet.rb ###
(注)未完成

予定ではWireshark等でキャプチャしたものをTsharkで変換テキストファイルを読み込むようにする予定。一種類のプロトコルについて一定時間ごとに区切りファイルに出力する。
 
	$ ruby read_in_packet 【入力ファイル名】 【出力ファイル名】

###sort_packet.rb###
(注)未完成

read_in_packetで生成したファイルを統合し、main.rbで使用できるファイルを生成する。現在は読み込むファイル数は3つであるが、今後第１引数で読み込むファイルの数を指定し好きな数読み込めるようにする予定。

	$ sort_packet.rb 【入力ファイル名】 【入力ファイル名】 【入力ファイル名】 【出力ファイル名】


パラメータの解説
----------------
リストの間に空行を挟むと、それぞれのリストに `<p>` タグが挿入され、行間が
広くなります。
 
    def MyFunction(param1, param2, ...)
 
+   `param1` :
    _パラメータ1_ の説明
 
+   `param2` :
    _パラメータ2_ の説明
 
