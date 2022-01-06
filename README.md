## ロボットシステム学　課題１

課題１としてmyled.cを作成しましたので添削よろしくお願いします。    

# プログラムの概要

　講義内で作成したmyled.cのプログラムを自分なりに改造し以下の動作をするように変更しました。  
 
 
　1.　約2秒停止。  
　2.　約10秒扇風機が回る。  
　3.　停止。  
# プログラムの使用手順
 _インストール_  
 $ git clone https://github.com/MatsuiYamato/robosys_motor.git  
 $ cd robosys_motor  
 $ make  
 $ sudo insmod myled.ko  
 $ sudo chmod a666 /dev/myled0
 
 _実行_  
 $ echo 1 > /dev/myled0  
 
 _アンインストール_  
 $ sudo rmmod myled  
 
# 工夫・アピール・改善点
　・電子回路を作成し、デジタル信号によってDCモータを動かせるようにした。
  ・実用性を考慮し、卓上扇風機を改造した。
  ・PWM制御にも挑戦したが、モータが回らなかったため断念した。
# 使用したもの
 * RaspberryPi4  
 * ブレッドボード  
 * ジャンパー線  
 * 抵抗  
 * LED  
 * トランジスタ
 * 卓上扇風機(DCモータ)
 * ダイオード
 
 # 実演動画
 https://youtu.be/KH6Zxg79mbg
 
 # ライセンス
 　GNU General Public License ver3.0
 
　


