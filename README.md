# flutter-dart
flutter-dart安装配置笔记


1、去官网下载flutterSDK，网站地址：[https://flutterchina.club/](https://note.youdao.com/)<br/>
2、解压SDK包到你想要放置的地址，如～ or 文稿 or /Applications<br/>
3、环境变量配置:MacOS环境变量配置<br/>

```
vim ~/.bash_profile（进入配置文件，i为输入 ESC 输入：wq为退出）

添加flutter环境变量一下语句：
export FLUTTER_HOME=flutter所在位置（为你放置flutter的文件夹地址）
export PATH=$PATH:$FLUTTER_HOME/bin
export PATH=$PATH:$FLUTTER_HOME/bin/cache/dart-sdk/bin

添加dart环境变量：
export PATH=${PATH}:/Users/aries/Flutter/flutter/bin/cache/dart-sdk/bin

flutter项目会依赖一些东西，在国内下载这些依赖会有一些慢，所以我们可以将它们的安装源换成国内的（也就是设置国内的镜像）
macOS或者Linux操作系统，依然是编辑~/.bash_profile文件
添加国内镜像变量：
export PUB_HOSTED_URL=https://pub.flutter-io.cn
export FLUTTER_STORAGE_BASE_URL=https://storage.flutter
注意： 此镜像为临时镜像，并不能保证一直可用，大家可以参考详情请参考 [https://flutter.dev/community/china](https://note.youdao.com/) 以获得有关镜像服务器的最新动态。

保存后退出，并在终端输入：
source ~/.bash_profile  //更新配置文件

检测是否配置成功：
dart --version
flutter --version
flutter doctor（可检测有哪些配置安装好，哪些配置没有安装）

```

4、关于VSCode插件的安装<br/>
```
1.flutter（必须）<br/>
2.dart（必须）<br/>
3.code runner（运行插件，可右键运行程序和使用快捷键）<br/>
```
5、如果发生如下错误，其实是VSCode dart代码没有Cmd+s保存，保存之后再运行错误消失
```
Dart_LoadScriptFromKernel: The binary program does not contain 'main'.

```
