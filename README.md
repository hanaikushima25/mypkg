# ロボットシステム学課題2

## 概要
2つのノードを動かし、二倍した結果を表示する

## 動作環境
- Raspberry Pi 4 Computer Model B
- OS:ubuntu 20.04 LTS
- ROS Noetic

## 実行手順
1.ディレクトリに入る
```
$ cd ~/catkin_ws/src
```
2.リポジトリをクローンする
```
$ git clone git@github.com:hanaikushima25/robosys_kadai2.git
```
3.一つ前のリポジトリに戻る
```
$ cd ..
```
4.コンパイルする
```
$ catkin_make
```
5.rosを起動する
```
$ roscore &
```
6.ディレクトリに入る
```
$ cd ~/catkin_ws/src/mypkg/scripts/
```
7.count.pyを実行する
```
$ chmod +x count.py   
$ roscore mypkg count.py
```
8.twice.pyを別の端末で実行する
```
$ chmod +x twice.py 
$ rosrun mypkg twice.py
```
9.また別の端末で実行する
```
$ rostopic echo /twice.py
```
停止する場合はctrl + c
## 実行結果
 Youtube https://www.youtube.com/watch?v=xc0hnqJGaRw
## 文責
 - Hana Ikushima
 - s20C1006NU@s.chibakoudai.jp
## ライセンス
　"mypkg" is under BSD 3-Clause "NEW" or "Revised"License.
 
 Thank you!
　

