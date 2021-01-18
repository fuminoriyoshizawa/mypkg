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
上田先生のhttps://github.com/ryuichiueda/ros_setup_scripts_Ubuntu20.04_server より以下を実行して、ROS環境を構築してください
```bash
$ ./step0.bash
$ ./step1.bash
```
次に以下を実行しワークスペースを準備して下さい。
```bash
$ mkdir -p catkin/src
$ cd ~/catkin_ws/src
$ catkin_init_workspace
```
次に以下を実行し
```bash
$ cd ~/catkin_ws/src
$ git clone 
