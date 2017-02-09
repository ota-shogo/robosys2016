#ロボットシステム学　課題 
###行ったこと
デバイスファイルにメッセージを送り、デバイスファイルからメッセージを出力。<br>
<iframe width="480" height="270" src="https://www.youtube.com/embed/vhDq4I0WyEE" frameborder="0" allowfullscreen></iframe>
###使い方<br>
事前にカーネルの再構築が必要。<br>
参考:https://github.com/ryuichiueda/raspberry_pi_kernel_build_scripts.git<br>
```
$git clone https://github.com/ryuichiueda/raspberry_pi_kernel_build_scripts.git
$cd raspberry_pi_kernel_build_scripts
$sudo ./kernal_build_and_install_for_pi2_pi3.bash
$sudo reboot
```
次にこのリポジトリーをクローンする。<br>
```
$git clone https://github.com/ota-shogo/robosys2016
```
実行する。
```
$cd robosys2016
$make
$sudo insmod myled.ko
$sudo cat /dev/myled0
```
次のコマンドをうち終了する。
```
CTRL + c
$sudo rmmod myled
```
##LISENSE<br>
ライセンスファイルを参照<br>
##REFERENCE
Ryuichi Ueda「CIT Autonomous Robot Lab」https://lab.ueda.asia/?page_id=1152, (last visit feb 9th,2017)<br>
Masaya Okawa「GitHub」 https://github.com/masamasa9841/robosys_2016_task, (last visit feb 9th, 2017)<br>
Masahiro Kato「GitHub」 https://github.com/kato-masahiro/RaspberryPi_LEDbrink, (last visit feb 8th,2017)<br>
