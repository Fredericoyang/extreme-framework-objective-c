[English](README_EN.md)
# 把极致带到开发中去

极致框架是一整套力求快速构建 iOS项目基本框架的完整解决方案，由核心框架、项目基本框架、核心UI以及核心工具集组成一个整体。项目基本框架基于核心框架封装快速解决基础问题，核心UI基于 Storyboard的封装，自动布局加持，摆脱代码定制烦恼，不断壮大的核心工具集满足常见功能速成方案的需要。

Hello world! 极致框架！

## 接入指南

1. Clone iOS项目基本文件到本地
2. 修改为自己的项目
3. 添加自己的项目文件，继续开发

> * [极致框架是什么](http://www.xfmwk.com/tags/极致框架/)
> * [快速上手](http://www.xfmwk.com/2019/05/22/快速上手目录/)
> * [开发文档](http://www.xfmwk.com/2019/05/22/开发文档目录/)
> * [常见问题](http://www.xfmwk.com/2019/05/22/常见问题/)

## 官网

打开 [官网](http://www.xfmwk.com/)

## 发布历史

### 正式版
#### 2.0(最终版) 2021-7-5
1       EFUtils: 转换工具添加了新的方法，添加了编码为 base64字符串和解码为 NSData的方法，UI工具添加了新的方法，取消了 DES加解密方法。
2       EFBase:
2.1     EFBaseViewController: 自定义返回与自定义取消方案改进，获取位置添加了新的方法，获取照片添加了新的方法，添加了获取录音权限的方法，添加了嵌入式 tableView的支持，可以像 EFBaseTableViewController中自带的 tableView一样使用，添加了数据刷新与分页和无数据显示的联动显示效果，输入聚焦方案改进。
2.2     EFBaseTableViewController: 自定义返回与自定义取消方案改进，获取位置添加了新的方法，获取照片添加了新的方法，添加了获取录音权限的方法，添加了数据刷新与分页和无数据显示的联动显示效果，输入聚焦方案改进。
2.3     EFBaseModalDialogViewController: 弹出式对话框基类，目前提供了最常用的三种弹出式对话框。
2.4     EFBaseWebViewController: UIWebView替换为 WKWebView。
2.5     BaseDataModel: 添加了自动归解档的支持。
3       EFUIKit:
3.1     EFNavigationBar: 取消了渐变色背景，深浅模式现在对应主题色，除了按钮、标题颜色，现在也作用于背景色。
3.2     EFModalDialog: 提供了最常用的三种弹出式对话框：列表单选或者多选、日期(时间可选)选择、最多两级的级联选项。
3.3     EFButton: 提供了边框、圆角、渐变背景自定义，内容水平居中、图标居左、图标居上多种显示风格。
3.4     EFView: 提供了边框、圆角、阴影效果自定义。
3.5     EFImageView: 提供了边框、圆角、阴影效果、图像填充方式自定义。
3.6     EFLabel: 提供了边框、圆角自定义，添加了通过 NSString实例化的方法，添加了文字显示不全时，点击以浮动提示方式显示全部文字的效果，默认不启用。
3.7     EFTextField: 提供了边框、圆角、占位文字颜色、文字显示位置偏移量自定义。
4       AFHTTPTool: AFHTTPConfig 错误码升级为状态码，获取 AFHTTPSessionManager时不再要求提供授权，改由各请求处理。
5       EFFMDBTool: 基于 BaseDataModel的模型sqlite自动存取。
6       演示 App同步更新，通过导航的深浅风格改变主题色。
7       适配了 iOS14系统，项目通过 Xcode12成功编译。

1.5(最终版) 2019-9-30
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
7	AppDelegate: 新增 App首次运行的 NSUserDefaults的配置项: init once。
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
优化了演示应用。兼容 Xcode10，基于最新 SDK编译。
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
