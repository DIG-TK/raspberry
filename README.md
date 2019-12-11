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

動作確認用　動画  
https://twitter.com/CitDaigo/status/1204627330116644864


# 参考資料
https://ryuichiueda.github.io/robosys2019/lesson7.html
