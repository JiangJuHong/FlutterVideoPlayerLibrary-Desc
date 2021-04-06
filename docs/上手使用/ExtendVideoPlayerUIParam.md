## ExtendVideoPlayerUIParam

`ExtendVideoPlayerUIParam`是对播放器可视化相关内容进行配置的类。

## 参数说明

| 参数名称                   | 参数类型 | 参数描述                                 | 常规默认值                       | 全屏默认值                       | 是否必传 |
| -------------------------- | -------- | ---------------------------------------- | -------------------------------- | -------------------------------- | -------- |
| luckButtonDisplay          | bool     | 是否显示锁定按钮                         | false                            | true                             |          |
| fullButtonDisplay          | bool     | 是否显示全屏按钮                         | true                             | false                            |          |
| returnButtonDisplay        | bool     | 是否显示返回按钮                         | 根据情况，如果有上一个页面则显示 | 根据情况，如果有上一个页面则显示 |          |
| moreButtonDisplay          | bool     | 是否显示更多按钮(请勿开启，功能暂未完善) | false                            | false                            |          |
| videoChangeButtonDisplay   | bool     | 是否显示分辨率切换按钮                   | false                            | true                             |          |
| playbackSpeedButtonDisplay | bool     | 是否显示倍速切换按钮                     | false                            | true                             |          |
| enabledGesture             | bool     | 是否启用手势控制                         | true                             | true                             |          |
| title                      | Widget   | 自定义标题                               |                                  | 常规默认值的内容                 |          |
| loading                    | Widget   | 自定义加载样式                           |                                  |                                  |          |
| returnIcon                 | Widget   | 自定义返回图标                           |                                  |                                  |          |
| moreIcon                   | Widget   | 自定义更多图标                           |                                  |                                  |          |
| indicatorIcon              | Widget   | 自定义进度指示器图标                     |                                  |                                  |          |

