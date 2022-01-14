# robosys_kadai2

## 概要
5つのノードを動かし、二倍三倍四倍した結果を表示する

## 動作環境
- Raspberry Pi 4 Computer Model B
- OS:ubuntu 18.04 LTS
- ROS Noetic

## 実行手順
```
1.ディレクトリに入る
$ cd ~/catkin_ws/src
2.リポジトリをクローンする
$ git clone https://github.com/yukikimuramura/robosys_2020_kadai02.git
3.一つ前のリポジトリに戻る
$ cd ..
4.コンパイルする
$ catkin_make
5.rosを起動する
$ roscore
6.ディレクトリに入る
$ cd ~/catkin_ws/src/robosys_2020_kadai02/scripts/
7.実行できるようにそれぞれのプログラムのパーミッションを設定する
$ chmod +x count.py       
$ chmod +x twice.py     
$ chmod +x three.py       
$ chmod +x four.py
8.count.pyを実行する
$ roscore mypkg count.py
9.twice.py,three.py,four.pyを実行する際それぞれ別の端末で実行する
$ rosrun mypkg twice.py
$ rosrun mypkg three.py
$ rosrun mypkg four.py
```
## 実行結果
## 文責
　- Hana Ikushima
　- s20C1006NU@s.chibakoudai.jp
　

