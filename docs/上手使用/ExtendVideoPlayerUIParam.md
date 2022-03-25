## ExtendVideoPlayerUIParam

`ExtendVideoPlayerUIParam`是对播放器可视化相关内容进行配置的类。

## 参数说明

| 参数名称                    | 参数类型 | 参数描述                            | 常规默认值                   | 全屏默认值                   | 必传 | 版本 |
|:---------------------------|:-------|:----------------------------------|:---------------------------|:---------------------------|:--------|----------------------------|
| volumeButtonDisplay        | bool     | 音量按钮是否显示，如果此内容为true，则会显示静音或非静音状态 | Web: true<br />Other: false      | Web: true<br />Other: false      |      | 1.1.0 |
| fullPlayerButtonDisplay    | bool     | 全屏播放按钮是否显示，如果此内容为true，则会在内容没有播放且没有锁定屏幕且没有显示操作菜单的时候显示。 | Web: true<br />Other: false      | Web: true<br />Other: false      |      | 1.1.0 |
| luckButtonDisplay          | bool     | 是否显示锁定按钮                                             | false                            | true                             | true | 1.0.0 |
| fullButtonDisplay          | bool     | 是否显示全屏按钮                                             | true                             | false                            | true | 1.0.0 |
| returnButtonDisplay        | bool     | 是否显示返回按钮                                             | 根据情况，如果有上一个页面则显示 | 根据情况，如果有上一个页面则显示 | true | 1.0.0 |
| moreButtonDisplay          | bool     | 是否显示更多按钮(请勿开启，功能暂未完善)                     | false                            | false                            | true | 1.0.0 |
| videoChangeButtonDisplay   | bool     | 是否显示分辨率切换按钮                                       | false                            | true                             | true | 1.0.0 |
| playbackSpeedButtonDisplay | bool     | 是否显示倍速切换按钮                                         | false                            | true                             | true | 1.0.0 |
| enabledGesture             | bool     | 是否启用手势控制                                             | true                             | true                             | true | 1.0.0 |
| title                      | Widget   | 自定义标题                                                   |                                  | 常规默认值的内容                 |      | 1.0.0 |
| loading                    | Widget   | 自定义加载样式                                               |                                  |                                  |      | 1.0.0 |
| returnIcon                 | Widget   | 自定义返回图标                                               |                                  |                                  |         | 1.0.0 |
| moreIcon | Widget | 自定义更多图标 | | | | 1.0.0 |
| indicatorIcon | Widget | 自定义进度指示器图标 | | | | 1.0.0 |

## 快速方法

你可以使用 `ExtendVideoPlayerUIParam.full` 和 `ExtendVideoPlayerUIParam.normal` 快速创建全屏和正常模式下的UI配置
