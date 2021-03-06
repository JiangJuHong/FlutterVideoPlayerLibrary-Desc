## 介绍

> 如果您不熟悉控制器的操作，请勿进行脏调用，避免出现预期之外的效果

### 可进行的操作

如果只是调试UI界面等功能不能满足您的业务需求，你还可以根据内部对象进行例如下面的操作：

* 控制视频功能(播放、暂停、跳转、切换分辨率、倍速等)
* 控制界面功能(显示或隐藏，全屏或非全屏)

### 控制器

此库中所有的控制操作均是使用`Model`来进行的，也就是说您可以通过调用`Model`中的方法或变更`Model`的参数来达到您想要的效果。

此库拥有如下几种控制器：

[ExtendVideoPlayerCoreModel](高阶使用/ExtendVideoPlayerCoreModel) 核心控制器

[ExtendVideoPlayerHooksModel](高阶使用/ExtendVideoPlayerHookModel) 钩子控制器

[ExtendVideoPlayerDrawerWindowModel](高阶使用/ExtendVideoPlayerDrawerWindowModel) 抽屉控制器

[ExtendVideoPlayerTipsModel](高阶使用/ExtendVideoPlayerTipsModel) 提示控制器

[ExtendVideoPlayerWindowModel](高阶使用/ExtendVideoPlayerWindowModel) 窗口控制器

### 获得控制器

为了防止控制器太多不利于维护，因此我们通过`ExtendVideoPlayerModelGroup`来对控制器进行集中管理，只要您获得了`ExtendVideoPlayerModelGroup`的引用，那么就能获得所有控制器。您可以通过以下案例来获得`ExtendVideoPlayerModelGroup`:

````dart
class VideoPlayerWidgetState extends State<VideoPlayerWidget> {
  /// 视频播放器全局key
  final GlobalKey<ExtendVideoPlayerState> _extendVideoPlayerKey = GlobalKey();

  void _getModelGroup(){
    ExtendVideoPlayerModelGroup modelGroup = _extendVideoPlayerKey.currentState.modelGroup;
  }
  
  @override
  Widget build(BuildContext context) {
    return ExtendVideoPlayer(
      key: this._extendVideoPlayerKey,
      resources: [
        ExtendVideoPlayerResource(url: "视频URL地址"),
      ],
      param: ExtendVideoPlayerParam(
        normalUIParam: ExtendVideoPlayerUIParam(returnButtonDisplay: false),
      ),
    );
  }
}
````

1. `GlobalKey<ExtendVideoPlayerState> _extendVideoPlayerKey = GlobalKey()` 定义全局Key，方便获取状态对象
2. `key: this._extendVideoPlayerKey`将全局Key引用传递给视频播放器
3. `ExtendVideoPlayerModelGroup modelGroup = _extendVideoPlayerKey.currentState.modelGroup`通过全局Key获得`ExtendVideoPlayerModelGroup`的引用

获得引用后，你可以分别使用以下代码来获得不同的管理器:

[ExtendVideoPlayerCoreModel](高阶使用/ExtendVideoPlayerCoreModel)

> modelGroup.manager

[ExtendVideoPlayerHooksModel](高阶使用/ExtendVideoPlayerHooksModel)

> modelGroup.hooksManager

[ExtendVideoPlayerDrawerWindowModel](高阶使用/ExtendVideoPlayerDrawerWindowModel) 

> modelGroup.drawerModel

[ExtendVideoPlayerTipsModel](高阶使用/ExtendVideoPlayerTipsModel) 

> modelGroup.tipsModel

[ExtendVideoPlayerWindowModel](高阶使用/ExtendVideoPlayerWindowModel) 

> modelGroup.windowModel

如果您想查看管理器的具体使用，请查看对应管理器的文档。

