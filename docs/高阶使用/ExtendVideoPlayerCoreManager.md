## ExtendVideoPlayerCoreManager

`ExtendVideoPlayerCoreManager` 是核心控制器，用于控制播放器相关内容

## 调用说明

| 名称               | 方法参数 / 属性类型       | 类型       | 描述                     | 使用                             |
| :----------------- | ------------------------- | ---------- | ------------------------ | -------------------------------- |
| loadResource       | Int index                 | 方法       | 加载资源(切换分辨率)     | model.loadResource(1)            |
| playIconController | AnimationController       | 属性       | 播放按钮动画控制器       | model.playIconController         |
| controller         | VideoPlayerController     | 属性       | 视频播放器控制器         | model.controller                 |
| isPlaying          | bool                      | 属性       | 是否播放中               | model.isPlaying                  |
| isBuffering        | bool                      | 属性       | 是否缓存中               | model.isBuffering                |
| value              | double                    | 属性       | 当前播放进度(秒)         | model.value                      |
| maxValue           | double                    | 属性       | 最大播放进度(秒)         | model.maxValue                   |
| error              | String                    | 属性       | 视频加载错误的信息       | model.error                      |
| pause              | -                         | 方法       | 暂停视频播放             | model.pause()                    |
| play               | -                         | 方法       | 恢复/开始 视频播放       | model.play()                     |
| seek               | Duration                  | 方法       | 跳转到指定时间节点       | model.seek(Duration(seconds: 0)) |
| index              | int                       | 属性       | 获得当前加载的资源的下标 | model.index                      |
| resource           | ExtendVideoPlayerResource | 属性       | 获得当前加载的资源       | model.resource                   |
| mainWindowSize     | Size                      | 属性       | 主窗口大小               | model.mainWindowSize             |
| full               | bool                      | 属性       | 是否全屏                 | model.full                       |
| full               | bool                      | 属性(设置) | 设置全屏                 | model.full = true                |
| uiParam            | ExtendVideoPlayerUIParam  | 属性       | 获得当前加载的UI参数     | model.uiParam                    |

