[English](README_EN.md)
#把极致带到开发中去

极致框架是一整套力求快速构建iOS项目基本框架的完整解决方案，由iOS项目基本框架、核心框架与核心UI组成一个整体。统一的宏与配置项，一处修改，全局生效，高效的工具方法类快捷解决基础问题，基于Storyboard的高度封装，自动布局加持，摆脱代码定制烦恼，高度封装的HTTPTool与高度集成于基类的方法满足常见需求速成方案的需要，集成式的工具箱囊括集成式支付、指纹验证、照片上传等常用集成功能模块。

Hello world! 极致框架！

![平台截图](http://www.xfmwk.com/images/folders_extreme_framework@2x.png)



## 接入指南

1. 从官方git地址Clone
1. 修改为自己的项目
1. 添加自己的项目文件，继续开发

> * [快速上手](http://www.xfmwk.com/2019/05/22/快速上手目录/)
> * [开发指南](http://www.xfmwk.com/categories/开发指南/)
> * [开发文档](http://www.xfmwk.com/categories/开发文档/)
> * [常见问题](http://www.xfmwk.com/categories/常见问题/)



## 官网

打开 [官网](http://www.xfmwk.com/)



## 发布历史

### 正式版

#### 1.5 2019-9-9
1	EFMacros: ROOT_VC调整，适用范围更广。
2	EFUtils:
2.1	新增了 boolValueFromNumber:，可快速从 NSNumber获取 boolValue。
2.2	新增了2个 NSDictionary的实用工具方法：将指定键值转换为字符串、判断指定键值是否与指定数值相等。
2.3	修复了2个 NSDictionary的实用工具方法结果有时不正确的问题：判断指定键值是否为空、判断所有键值是否存在空。
3	EFBase:
3.1	EFNavigationBar深色模式除了按钮颜色，现在也作用于标题颜色。
3.2	EFBaseViewController/EFBaseTableViewController: 
3.2.1	新增使用位置授权的独立方法，并解决了使用位置授权弹框很久才显示的问题。
3.2.2	改进了控制器自定义返回和自定义取消的处理逻辑，支持随时开关，可先自定义返回按钮/自定义取消按钮。
3.2.3	优化了照片选择器，现支持拍照时默认前置摄像头。
3.3	EFBaseWebViewController: 初始加载时标题显示页面加载中。现在关闭按钮能及时显示了。
3.4	BaseDataModel: dataID和 dataName不再要求必须提供。
4	ImageUploadTool: 支持自定义图片上传接口路径和用于自定义图片上传接口的 image Key，并可自定义上传时的提示信息。
5	AppConfig: 归类并增加说明，更有条理。
6	AppMacros: Theme Colors配置项移至 AppConfig。
7	AppDelegate: 新增App首次运行的 NSUserDefaults的配置项: init once。
8	请求位置信息另外添加了总是使用位置的隐私权限描述。
9	同步改进的演示App，集成 AFHTTPTool的演示。
10	彩蛋：登录界面图标连续点击切换服务器环境，仅开发测试有效。

1.4 2019-6-13
AFHTTPTool：直接通过 AFHTTPConfig配置自定义项，优化的错误分级处理。

1.3 2019-5-16
1、全新 EFUIKit，新增集成于控制器基类(EFBaseViewController和 EFBaseTableViewController)中的直接访问基于 EFNavigationBar的导航栏的能力，现在可以直接设置导航栏的渐变色背景，和深浅风格(作用于导航栏上的按钮)。
2、演示优化：扫一扫现可重复扫描，应用于更多的场景。
3、项目目录结构优化，开发与组织更加平衡。

1.2 2019-2-20
基于控制器基类封装的相机、照片访问的权限处理方法现已可独立调用。
新增 CodeScanerTool: 扫一扫。

1.1.2 2018-10-09
修复了基于表格控制器基类中封装的 MJRefresh启用之后再自定义 refreshHeader和 refreshFooter无效的问题。

1.1.1 2018-9-20
优化了演示应用。兼容 Xcode10，基于最新SDK编译。
新增：
1、EFUtils: DES加解密的相关方法，适用于常规加解密。
2、LABiometryTool: iPhone X面容验证。
3、适应苹果政策完善权限描述。

1.1 2018-7-25
修复：
1、修复集成于控制器基类中的没有允许定位第二次请求定位不走回调的问题。
2、WebTool: 修复了 WebTool中点击某些特殊的链接加载视图会一直显示的问题。
新增：
1、演示应用。
2、基于表格控制器基类中封装的 MJRefresh，简化基于表格控制器基类中封装的 MJRefresh的使用。注意子类中方法的重写(loadData和 loadMoreDataWithPageNumber:)。
3、集成于控制器基类中的全新的自定义的返回按钮，不仅支持导航按钮自由组合使用，还能自定义方法，同时保持原有手势返回的特性。
4、集成于控制器基类中的全新的自定义的取消按钮，不仅支持导航按钮自由组合使用，还能自定义方法。

1.0 2017-8-1
特色：
1、控制器基类封装多种常用功能，使用方便快捷。
2、导航控制器基类新增透明导航风格。
3、用于 Storyboard中导航的自定义标题视图和按钮自定义视图。
4、各种常用工具组件，接口调用、图片上传、本地生物特征验证、Web内容访问，后续会加入更多的工具组件。
5、统一的配置项、宏与工具类，开发更高效。