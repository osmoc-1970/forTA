## Cloud9の作業環境の調整

このコースで利用しやすくするために、以下の手順でCloud9のチューニングを行ってください。

チューニングの概要は以下のようになります（内容は深く知らなくて結構です。）
- WordPressコースで使わないdockerイメージの削除
- EBS（ストレージ領域）の拡張
- OSが確保するキャッシュメモリを解放
- swap領域（メインメモリーの一時退避領域）の拡張

```
これは必ず実施してください。実施しないと、この後のレッスンでディスク容量不足になり様々な問題が発生します。
```


### チューニング作業手順

(1) シェルスクリプトファイルを下記のリンクよりダウンロードします。

(cloud9tuning.shファイルのリンク)

(2)ダウンロードができたら、AWS Cloud9の左ファイルツリーの一番上のフォルダ（WordPress_ で始まるフォルダ）をクリックして選択してから、「File」から Update Local Files... を選択してください。

![アップロード手順画像](https://techacademy.s3.amazonaws.com/bootcamp/lessons/orientation/cloud9_wordpress_4.png)

選択すると「Upload Files」のウィンドウが表示されます。

![アップロード手順画像](https://s3-ap-northeast-1.amazonaws.com/techacademy-bootcamp/pictures/428/original.png)

ここで、 Select files をクリックし、さきほどダウンロードしたcloud9tuning.shを選択してください。

(3)アップロードした cloud9tuning.sh を実行します。ターミナルウィンドウを開きます。「AWS Cloud9の基本的な使い方」でターミナルを開く手順を説明しています。

ターミナルウィンドウを開いたら、下記のコマンドを入力します。

```
bash cloud9tuning.sh
```

数十秒かかるとコマンドが終了します。これで完了です。

https://gyazo.com/df8c06601e867f8d05c142d36d875b2c

![完了画面](https://i.gyazo.com/df8c06601e867f8d05c142d36d875b2c.png)
