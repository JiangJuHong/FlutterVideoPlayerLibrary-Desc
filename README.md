# 什么是 video_player_library

video_player_library 是 Flutter 平台的视频播放器库，播放器核心基于 [video player](https://pub.dev/packages/video_player) 。内置功能丰富，方便您的项目完成快速交付。

> 注：部分功能不支持模拟器上运行，实际效果以真机为准。

[点击查看使用文档](https://video-player.docs.huic.top)


# 优势

* 快速集成：参考文档两分钟即可接入到你的项目。
* 功能丰富：支持`多源视频加载`、`窗口/全屏模式`、`清晰度切换`、`倍速切换`、`手势控制`、`横竖屏`、`音量控制`、`亮度控制`、`自定义组件`、`自定义钩子`等功能
* 持续维护：项目会持续迭代，功能会越来越丰富。如果某个功能存在缺陷，将会在最短的时间内进行修复。
* 跨平台性：项目支持Android、IOS、Web(Mobile)
* 插件兼容：支持Flutter 2.0，空安全

## 项目截图

<img
src="https://github.com/JiangJuHong/access-images/blob/master/FlutterVudeoPlayerLibrary/1.png"
height="300em" />
<img
src="https://github.com/JiangJuHong/access-images/blob/master/FlutterVudeoPlayerLibrary/2.png"
height="300em" style="max-width:100%;display: inline-block;"/>
<img
src="https://github.com/JiangJuHong/access-images/blob/master/FlutterVudeoPlayerLibrary/3.png"
height="300em" style="max-width:100%;display: inline-block;"/>

## 项目视频

[点我查看(Demo)](https://dev-storage.huic.top/video_player_library/Video/Demo.mp4)  
[点我查看(线上项目)](https://dev-storage.huic.top/video_player_library/Video/%E8%B6%B3%E8%B6%A3%E7%A4%BE%E5%8C%BA.mp4)  

## Demo下载

> 由于Demo无法上架，故仅支持Android Demo下载。

<img src="https://github.com/JiangJuHong/access-images/blob/master/FlutterVudeoPlayerLibrary/code.png" style="display: inline-block;"/>

## 使用文档

[点击查看使用文档](https://video-player.docs.huic.top)

## 功能与定价

购买链接: [点击这里](http://wpa.qq.com/msgrd?v=3&uin=690717394&site=qq&menu=yes)  
联系客服: [点击这里](http://wpa.qq.com/msgrd?v=3&uin=690717394&site=qq&menu=yes)

| 功能列表           | 专业版 |
| :----------------- | :----- |
| 视频播放           | ✅      |
| 倍速播放           | ✅      |
| 窗口模式           | ✅      |
| 全屏模式           | ✅      |
| 多清晰度无感切换   | ✅      |
| 横竖屏切换         | ✅      |
| 手势控制           | ✅      |
| 长按快进           | ✅      |
| 音量控制           | ✅      |
| 亮度控制           | ✅      |
| 自定义指示器图标   | ✅      |
| 自定义加载进度样式 | ✅      |
| 钩子操作         | ✅    |
| 锁定               | ✅      |
| 价格               | 288    |

## 结尾

为什么会有这个项目？

> 答：由于之前重复编写过很多系统的视频播放器，也逐一踩过不少坑，因此专门花了一大段时间来编写这个项目，把踩过的坑都避免，封装一个近乎完美的视频播放器。

为什么会收费？

> 答：由于本人目前是自由职业，收入来源有限，故打造一类收费版的插件，一来维持生活，二来能够制作更精心的内容。

这个维护得怎么样？

> 答：1. 出现BUG第一时间修复，修复后紧急发布。
>
> 答：2. 持续收集大家的建议，一直迭代该产品。

我有不明白的怎么办？

> 答：如果您在集成中有任何不明白，可以通过向群内问答，热心的开发者以及我本人会在第一时间进行回复。

还有其它想说的吗？

> 答：感谢大家的围观，欢迎关注我的[Github](https://github.com/JiangJuHong)账号。


## 版本变更
### 1.1.1(Dev)

* 增加: ExtendVideoPlayerResource 支持传递 VideoFormat（仅对network视频有效）
* 增加: 资源播放失败后将自动切换资源
* 移除: auto_orientation 组件，使用 SystemChrome.setPreferredOrientations 实现横竖屏切换
* 调整: 代码结构调整，将 model 从 entitys 里面抽出

### 1.1.0 (2021-09-22)

* 调整: 播放图标大小
* 增加: ```volumeButtonDisplay``` 属性控制音量按钮是否显示(web默认为true，其它默认为false)。此属性可以控制是否静音
* 增加: ``fullPlayerButtonDisplay`` 属性控制全屏播放按钮是否显示，(web默认为true，其它默认为false)
* 增加: **web端支持**(移动端web，暂不支持pc web)
* 增加: debug日志输出
* 修复: 部分时长显示异常问题

### 1.0.1

* 增加钩子，增加权限钩子
* 权限钩子: 播放源切换、全屏切换

### 1.0.0
* 全屏/窗口模式
* 倍速播放
* 分辨率切换
* 锁定窗口
* 自定义标题
* 自定义进度条
* 自定义加载动画
* 空安全