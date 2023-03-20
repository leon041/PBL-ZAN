# 防犯カメラシステム[ZAN]

不審者がカメラに映ると自動で撮影し、GooglDrive上に保存、LINEに通知される

# 回路図とシステム概形
* 回路図
![実験接続図](https://user-images.githubusercontent.com/112361650/226249517-0b1970e9-e467-412f-a9ce-8ccae870e665.png)

* システム概形図
![システム概形図](https://user-images.githubusercontent.com/112361650/226249505-96b12e9c-97e1-479d-b6be-c31cf3940f09.png)

# 使用したもの

* OMRON TYPE GLS-M1(磁気センサ)  :  1組
* 抵抗1000Ω(誤差±５%)   : １つ
* Raspberry Pi Camera V2.1  :  １つ
* ブレッドボード  :  1つ
* ワニーワニ導線  :  2本
* 導線 : 6本
* LINE MESSAGING API : LINE BOT開発用API
* Google Drive API : Google Driveの操作用API
* heroku: Cloud(PaaS)サービス

# ライブラリ
* Flask(1.0.2) : webサーバー用
* line-bot-sdk(2.0.1) : LINE Messaging API用 
* PyDrive(1.3.1) : Google Drive API用
* RPi.GPIO(0.7.0) : GPIO制御用
* requests(2.21.0) : httpの通信用のライブラリ

# 実際の動作
# RPi側ログ 
![ログ1](https://user-images.githubusercontent.com/112361650/226249508-2b07c385-c020-41ba-b88a-197d049d5eb1.png)
![ログ2](https://user-images.githubusercontent.com/112361650/226249514-441b5383-670e-4ac5-a703-f4becfd3a102.png)

# サーバー側ログ 
![ログ3](https://user-images.githubusercontent.com/112361650/226251427-fdb2e8cb-34ed-481f-94e0-3cf38fae80b4.png)

# 通知
![通知](https://user-images.githubusercontent.com/112361650/226249525-2c668cef-d834-4dbc-ad4a-8d58fab21a31.png)

# コマンド 
![コマンド](https://user-images.githubusercontent.com/112361650/226249468-88d33b7d-28d1-4b23-baf7-ddbf344c4760.jpg)
* count 	: ドアが開いた総回数取得
* date		: ドアが開いた日時のリストと回数の取得
* YYYY-MM-DD: 指定された日付のドアカウントの取得
* NUMBER	: 指定されたドアカウントの代表的な写真を取得
* それ以外 : ヘルプ
  
  
# 取得 
![取得](https://user-images.githubusercontent.com/112361650/226249520-7e8a84e7-d31c-4dd5-ba82-fa23fd542da7.jpg)

