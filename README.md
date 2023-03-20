# 防犯カメラシステム[ZAN]

不審者がカメラに映ると自動で撮影し、GooglDrive上に保存、LINEに通知される

# 回路図とシステム概形



# 使用したもの

*　OMRON TYPE GLS-M1(磁気センサ)  :  1組
*　抵抗1000Ω(誤差±５%)   : １つ
*　Raspberry Pi Camera V2.1  :  １つ
*　ブレッドボード  :  1つ
*　ワニーワニ導線  :  2本
*　導線 : 6本
*　LINE MESSAGING API : LINE BOT開発用API
*　Google Drive API : Google Driveの操作用API
*　heroku: Cloud(PaaS)サービス

# ライブラリ
* Flask(1.0.2) : webサーバー用
* line-bot-sdk(2.0.1) : LINE Messaging API用 
* PyDrive(1.3.1) : Google Drive API用
* RPi.GPIO(0.7.0) : GPIO制御用
* requests(2.21.0) : httpの通信用のライブラリ

