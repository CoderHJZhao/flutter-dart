# flutter-dart
flutter-dart安装配置笔记


1、去官网下载flutterSDK，网站地址：[https://flutterchina.club/](https://note.youdao.com/)<br/>
2、解压SDK包到你想要放置的地址，如～ or 文稿 or /Applications<br/>
3、环境变量配置:MacOS环境变量配置<br/>

```
vim ~/.bash_profile（进入配置文件，i为输入 ESC 输入：wq为退出）

添加flutter环境变量一下语句：
export FLUTTER_HOME=/Applications/flutter（为你放置flutter的文件夹地址）
export PATH=$PATH:$FLUTTER_HOME/bin
export PATH=$PATH:$FLUTTER_HOME/bin/cache/dart-sdk/bin

添加dart环境变量：
export PATH=${PATH}:/Users/aries/Flutter/flutter/bin/cache/dart-sdk/bin

保存后退出，并在终端输入：
source ~/.bash_profile  //更新配置文件

检测是否配置成功：
dart --version
flutter doctor

```
