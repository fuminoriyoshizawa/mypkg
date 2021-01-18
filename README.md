# robotsystems-task2
ロボットシステム学課題2
# 概要
講義内で作成したプログラムを、ライセンスを整備して動かしました。
変更点はありません。
# 環境
* Raspberry Pi4 ModelB 4GB
* Ubuntu20.04
* ROS Noetic
# プログラムのインストール
上田先生のhttps://github.com/ryuichiueda/ros_setup_scripts_Ubuntu20.04_server より以下を実行して、ROS環境を構築して下さい。
```bash
$ ./step0.bash
$ ./step1.bash
```
次に以下を実行してプログラムのインストールとビルドを行って下さい。
```bash
$ mkdir -p catkin/src
$ cd ~/catkin_ws/src
$ catkin_init_workspace
$ cd ~/catkin_ws/src
$ git clone https://github.com/fuminoriyoshizawa/mypkg.git
$ cd ~/catkin_ws
$ catkin_make
$ source ~/.bashrc
```
# 動作確認
ターミナルを4つ開き、それぞれの端末に順番に以下のコマンドを入力し、動作を確認して下さい。
```bash
$ roscore                     //端末1に入力
$ rosrun mypkg count.py       //端末2に入力
$ rosrun mypkg twice.py       //端末3に入力
$ rostopic list               //端末4に入力し roscore、count.py、twice.pyが動作しているか確認
$ rostopic echo /twice        //端末4に入力
```
# 動作の様子
以下のリンクから実際の動作状況が確認できます。
* 
