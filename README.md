# RS1
ロボットシステム学の課題１のリポジトリである。  

# 概要
講義内で作成したプログラムを参考に自身で改造し、LEDを3個に増やしてそれぞれ点滅させることが出来るプログラム。  

# 使用したもの  
・Ubuntu18.04　LTS  
・Raspberry Pi 4  
・LED×3  
・抵抗×3  
・ジャンパー線×3  
・ブレッドボード  

# 動作方法  
・ビルド  

    $ make  
    $ sudo insmod myled.ko  
    $ sudo chmod 666 /dev/myled0  
・実行  

    $ echo 1 > /dev/myled0 (1つ目のLEDを光らせる)  
    $ echo 3 > /dev/myled0 (2つ目のLEDを光らせる)  
    $ echo 5 > /dev/myled0 (3つ目のLEDを光らせる)  
    $ echo 0 > /dev/myled0 (1つ目のLEDを消す)  
    $ echo 2 > /dev/myled0 (2つ目のLEDを消す)  
    $ echo 4 > /dev/myled0 (3つ目のLEDを消す)  
  
# 動画  
https://youtu.be/ean9h4ObPDM  

# ライセンス  
https://github.com/Ryo12345678/RS1/blob/8244011524f3597fd455bbf4b6fbff438ceff888/COPYING
