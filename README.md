# robosys_kadai2

## 概要
2つのノードを動かし、二倍した結果を表示する

## 動作環境
- Raspberry Pi 4 Computer Model B
- OS:ubuntu 20.04 LTS
- ROS Noetic

## 実行手順
```
1.ディレクトリに入る
$ cd ~/catkin_ws/src
2.リポジトリをクローンする
$ git clone git@github.com:hanaikushima25/robosys_kadai2.git
3.一つ前のリポジトリに戻る
$ cd ..
4.コンパイルする
$ catkin_make
5.rosを起動する
$ roscore &
6.ディレクトリに入る
$ cd ~/catkin_ws/src/mypkg/scripts/
7.実行できるようにそれぞれのプログラムのパーミッションを設定する
$ chmod +x count.py       
$ chmod +x twice.py     
8.count.pyを実行する
$ roscore mypkg count.py
9.twice.pyを別の端末で実行する
$ rosrun mypkg twice.py
```
## 実行結果
 Youtube https://www.youtube.com/watch?v=xc0hnqJGaRw
## 文責
  - Hana Ikushima
　- s20C1006NU@s.chibakoudai.jp
## ライセンス
　"mypkg" is under GNU General Public License v3.0.
 
 Thank you!
　

