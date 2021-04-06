## ExtendVideoPlayer

`ExtendVideoPlayer`是播放器主类，通过此播放器进行UI显示，控制播放等功能。

## 参数说明

| 参数名称     | 参数类型                                                     | 参数描述           | 默认值                   | 是否必传 |
| ------------ | ------------------------------------------------------------ | ------------------ | ------------------------ | -------- |
| param        | [ExtendVideoPlayerParam](上手使用/ExtendVideoPlayerParam.md) | 播放器自定义参数   | ExtendVideoPlayerParam() |          |
| resources    | List\<[ExtendVideoPlayerResource](上手使用/ExtendVideoPlayerResource.md)> | 视频资源           |                          | 是       |
| defaultIndex | int                                                          | 默认播放视频的下表 | 0                        |          |
| full         | bool                                                         | 是否开启全屏模式   | false                    |          |