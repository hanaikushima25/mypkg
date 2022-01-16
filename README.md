# ロボットシステム学課題2

## 概要
2つのノードを動かし、二倍した結果を表示する

## 動作環境
- Raspberry Pi 4 Computer Model B
- OS:ubuntu 20.04 LTS
- ROS Noetic

## 実行手順
1.ディレクトリを作成する
```
 cd 
 mkdir -p catkin_ws/src
 cd ~/catkin_ws/src
 catkin_init_workspace
```
2. .bashrcの下から三行目に以下の文を入れる
```
 source ~/catkin_ws/devel/setup.bash
```
3.環境のビルドをする
```
 cd ~/catkin_ws
 catkin_make
 source ~/.bashrc
```
4.パッケージを作成する
```
 cd ~/catkin_ws/src
 catkin_create_pkg mypkg rospy
```
5.パッケージ内にscriptsというディレクトリを作成し、ノードとなるプログラムを置く
```
 cd mypkg/
 mkdir scripts
 cd scripts/
```
6.ROSを立ち上げる
```
 roscore &
```
7.count.pyを実行する
```
 chmod +x count.py   
 roscore mypkg count.py
```
8.twice.pyを別の端末で実行する
```
 chmod +x twice.py 
 rosrun mypkg twice.py
```
9.また別の端末で実行する
```
 rostopic echo /twice.py
```
停止する場合はctrl + c
## 実行結果
 Youtube https://www.youtube.com/watch?v=xc0hnqJGaRw
## 文責
 - Hana Ikushima
 - s20C1006NU@s.chibakoudai.jp
## ライセンス
　"mypkg" is under BSD 3-Clause "NEW" or "Revised"License.
 
## 参考
　https://ryuichiueda.github.io/robosys2020/lesson10_ros.html#/20
 
 Thank you!
　

