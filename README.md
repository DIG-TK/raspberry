### ロボットシステム学
raspberryPi3を使用してLEDを点滅させる

# 実行方法

LEDの点滅

`$make`  
`$sudo insmod myled.ko`  
`$sudo chmod 666 /dev/myled0`  
`$echo 1 > /dev/myled0		# LEDを点灯`  
`$echo 0 > /dev/myled0		# LEDを消灯`  

ログの確認

`$tail /var/log/messages`  
`[  1162.919529]LED_ON`  
`[  1170.558968]LED_OFF`  

デバイスファイルを消す

`$sudo rmmod myled`  

# 参考資料
動作確認用　動画  
[google]https://twitter.com/CitDaigo/status/1202463610796044288
