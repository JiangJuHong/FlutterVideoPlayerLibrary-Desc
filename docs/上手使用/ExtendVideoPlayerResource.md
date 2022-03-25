## ExtendVideoPlayerResource

`ExtendVideoPlayerResource`是播放器对视频资源进行封装的类。

## 参数说明

| 参数名称 | 参数类型 | 参数描述                                            | 默认值 | 是否必传 | 版本 |
|:-------|:--------|:--------------------------------------------------|:------|:-------|--------|
| id     | String  | 资源ID，使用者自定义                                 |       |         | 1.0.0 |
| url    | String  | 视频网络地址                                        |       |         | 1.0.0 |
| asset  | String  | 视频Asset地址                                       |      |         | 1.0.0 |
| file   | Stirng  | 视频文件路径                                        |       |         | 1.0.0 |
| label  | String  | 文本标签(如果您开启了切换分辨率功能，此属性则代表分辨率名称) |       |        | 1.0.0 |
| formatHint | VideoFormat | 视频格式，仅当视频为网络URL时有效 | | | 1.1.0 |

