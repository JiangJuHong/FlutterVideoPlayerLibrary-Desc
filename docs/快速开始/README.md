## 购买

如果您未购买此项目，请联系[客服](http://wpa.qq.com/msgrd?v=3&uin=690717394&site=qq&menu=yes)进行购买。

## 下载

如果您已经购买了项目，请使用解压缩工具将`FlutterVideoPlayerLibrary.zip`进行解压缩

## 安装

请确保您的项目为Flutter项目。此插件仅支持Flutter项目。

### 导入库文件

1. 假设您的项目结构为:

   ````
   {project_name}/
   	android
   	ios
   	lib
   	test
   	pubspec.yaml
   ````

2. 请在项目根路径创建文件夹`library`，当然，您也可以使用任意未存在的字符串代替。

3. 创建目录完成后，请将库文件移动到`library`，移动结束后您的项目结构应该为:

   ````
   {project_name}/
   	android
   	ios
   	lib
   	test
   	library
     	FlutterVideoPlayerLibrary
     		lib
         library  		
     		pubspec.yaml
     		.metadata
   	pubspec.yaml
   ````

   >  由于版本迭代关系，不同版本FlutterVideoPlayerLibrary内的目录结构可能不同。

4. 当库成功被移动到您的项目当中后，请打开您的项目的 `pubspec.yaml` 文件，更改 `dependencied`部分为

   ````yaml
   dependencied:
   	...
   	video_player_library:
     	path: library/FlutterVideoPlayerLibrary
   ````

   > 注: `...`代表您项目原有依赖。

   至此，您的项目已成功集成 `FlutterVideoPlayerLibrary`

### 更新依赖

当库成功导入到项目后，您还不能使用，您还需要：

1. 如果您是使用 `Idea/Android Studio` 进行开发，请进入`pubspec.yaml`文件，并点击窗口右上角的`Pub get`
2. 如果您使用的是其它Ide，请通过命令行进入到项目根目录，然后执行: `flutter pub get`



### 使用

接下来，您可以正式进入使用环节，请点击[使用文档](上手使用/README.md)继续阅读。