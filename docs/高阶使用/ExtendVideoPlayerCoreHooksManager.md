## ExtendVideoPlayerCoreHooksManager

`ExtendVideoPlayerCoreHooksManager` 是钩子控制器，用于对播放器操作控制或记录监听。

钩子的使用很简单，你只需要获得钩子管理器后进行注册/移出钩子即可，关于如何获得钩子管理器，请参考:[获得控制器](./README.md#获得控制器)。

当获得钩子管理器后可以执行注册/移出钩子操作，示例代码(以权限钩子为例):

````dart
/// 自定义权限钩子
class CustomPermissionsHook extends PermissionsHook{
  
  	/// 当此方法返回false时，将不允许本次权限，那么就无法进行设置全屏操作
  	@override
    bool changeFull(bool full) => false;
}

class Main{
  CustomPermissionsHook hook = CustomPermissionsHook();
  
  /// 注册钩子
 	void reg(){
  	_hooksManager.registerHook(hook);
	} 
  
  /// 移出钩子
  void remove(){
    _hooksManager.removeHook(hook);
  }
}

````

> 不同的钩子类型将提供不同的操作，例如权限控制钩子是允许你对操作进行限制，比如是平台VIP才能进行切换播放源，就可以通过权限控制钩子对非VIP进行限制。

目前支持的钩子类型:

`PermissionsHook` 

> 权限控制钩子，用来对操作进行限制，例如：允许/禁止全屏，允许/禁止切换分辨率。
>
> 权限控制钩子中，所有方法的返回值均是 bool，代表是否允许执行此操作，返回true代表允许，返回false代表不允许。

| 方法名称             | 参数描述                                                     | 方法描述            |
| :------------------- | :----------------------------------------------------------- | :------------------ |
| changePlaybackSource | ExtendVideoPlayerResource oldResource: 正在播放的资源<br />ExtendVideoPlayerResource newResource: 目标资源 | 切换播放源时触发    |
| changeFull           | bool full: 是否是全屏                                        | 切换/取消全屏时触发 |