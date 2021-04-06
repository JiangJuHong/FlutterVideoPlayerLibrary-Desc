## 简单案例

### 简单案例

将以下代码复制到您项目中，并将URL替换为可用的URL：

> 注: 创建视频播放器，并指定一个资源，资源来源为URL

````dart
ExtendVideoPlayer(
  resources: [
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4"),
  ],
)
````

执行 `flutter run`，您将看到一个小型视频窗口

<img src="images/small_window.png" width="300px"/>

### 如果您想指定视频标题，则可以进行如下配置: 

````dart
ExtendVideoPlayer(
  resources: [
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4"),
  ],
  param: ExtendVideoPlayerParam(
  	normalUIParam: ExtendVideoPlayerUIParam(
    	title: Text("我是视频标题"),
    ),
  ),
)
````

### 如果您想设置多分辨率，则可以进行如下配置：

````dart
ExtendVideoPlayer(
  resources: [
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4", label: Text("超清")),
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4", label: Text("高清")),
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4", label: Text("清晰")),
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4", label: Text("流畅")),
  ],
  param: ExtendVideoPlayerParam(
  	normalUIParam: ExtendVideoPlayerUIParam(
    	title: Text("我是视频标题"),
    ),
  ),
)
````

### 如果您想禁用手势和禁用全屏按钮，则可以进行如下配置:

````dart
ExtendVideoPlayer(
  resources: [
    ExtendVideoPlayerResource(url: "https://dev-storage.huic.top/video_player_library/Video/Demo.mp4"),
  ],
  param: ExtendVideoPlayerParam(
  	normalUIParam: ExtendVideoPlayerUIParam(
    	enabledGesture: false,
      fullButtonDisplay: false,
    ),
  ),
)
````

> 效果实现了，如果你想指定更多参数，可以参考: [ExtendVideoPlayer](上手使用/ExtendVideoPlayer.md)。