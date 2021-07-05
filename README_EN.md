[中文](README_CN.md)
# Brings Extreme To Development

The ExtremeFramework is a complete solution to quickly create the iOS project basic files, which is composed of the core framework, the basic folders and files of project, the core UI kit and the core tool kit. The basic folders and files of project is based on the core framework to quickly solve the basic problems. The core UI kit is based on the Storyboard, and the autolayout, it's so easy to customize without code programming. The core tool kit greater than ever to use common function quickly and easily.

Hello world! ExtremeFramework！

## Access Guide

1. Clone the iOS project basic files
2. Modify it to your own project
3. Add your own project files and continue to development

> * [ExtremeFramework Is What](http://www.xfmwk.com/tags/极致框架/)
> * [Quick Start](http://www.xfmwk.com/2019/05/22/快速上手目录/)
> * [Documents](http://www.xfmwk.com/2019/05/22/开发文档目录/)
> * [FAQ](http://www.xfmwk.com/2019/05/22/常见问题/)

## Official Website

Open [Official Website](http://www.xfmwk.com/)

## Release History

### Release

#### 2.0(Definitive Edition) 2021-7-5
1 EFUtils: The conversion utils gets new methods to encode NSData to Base64 strings and decode NSData from them. New methods for UI utils. The DES encryption and decryption method is removed.
2 EFBase:
2.1 EFBaseViewController: Custom back and custom cancel solution improvements, new methods for request locations, new methods for select photos, new method for request recording permission, and embedded tableView is supported, just use like the EFBaseTableViewController own tableView, data refresh and pageable with display no data view during animations, solution of input focus improvement.
2.2 EFBaseTableViewController: Custom back and custom cancel solution improvements, new methods for request locations, new methods for select photos, new method for request recording permission, data refresh and pageable with display no data view during animations, solution of input focus improvement.
2.3 EFBaseModalDialogViewController: Modal dialog base class, now provides the most commonly used three modal dialog.
2.4 EFBaseWebViewController: Replace UIWebView with WKWebView.
2.5 BaseDataModel: Added support for archive and unarchive automatic .
3 EFUIKit:
3.1 EFNavigationBar: The gradient background is removed. The navigation style is applied by the theme color. In addition to the bar button item and title color, it also applied to the background color.
3.2 EFModulalDialog: It provides the three most commonly used modal dialogs: list option with single or multiple selection, select date(or date and time), and level-able options up to two levels.
3.3 EFButton: Customized border, corner radius, and gradient background. it provides a lot of display styles such as horizontal content center, icon on the left and icon on the top.
3.4 EFVIEW: Customized border, corner radius or shadow.
3.5 EFImageView: Customized border, corners radius or shadow, and image content mode.
3.6 EFlabel: Customized border, corners radius, it provides a lot of methods to init label with NSString, and display all text in pop-over view when the text is not displayed completely just simply by a single tap.
3.7 EFTextField: Customized border, corner radius, placeholder text color, and text display position offset.
4 AFHTTPTool: The AFHTTPConfig error code is upgraded to status code, and authorization is no longer required when get AFHTTPSessionManager, just handle by each request instead.
5 EFFMDBTool: Read from or save to sqlite automatic just by models based on BaseDataModel.
6 The demo App is upgraded at the same time, and the navigation style is applied by the theme color.
7 Compatible with iOS 14, and the project is successfully compiled by Xcode12.

1.5(Definitive Edition) 2019-9-30
1 EFMacros: ROOT_VC adjustment, applicable to a wider range.
2 EFUtils:
2.1 there is a new utility method boolValueFromNumber:, which can quickly get the boolValue from the NSNumber.
2.2 two new NSDictionary utility methods are added: convert the specified key value to a string and determine whether the specified key value is equal to the specified value.
2.3 fixes problems with two NSDictionary utility methods that sometimes result in incorrect results: determining whether the specified key value is empty, and determining whether key value in dictionary might be null.
3 EFBase:
3.1 EFNavigationBar dark mode now available on the title and the bar button item both.
3.2 EFBaseViewController/EFBaseTableViewController:
3.2.1 add an independent method to use location authorization, and and solve the problem of display using location authorization alert sheet for elapsed a long time.
3.2.2 improved the processing logic of the controller's custom back and custom cancel. It supports switching at any time. You can customize the back button/custom cancel button first.
3.2.3 optimized photo selector, now supports the default front-camera when taking photos.
3.3 EFBaseWebViewController: the title "页面加载中" is displayed when the page is initial loading. The "关闭" button now shows up in time.
3.4 BaseDataModel: dataID and dataName are no longer required to be provided.
4 ImageUploadTool: supports the custom URL of the image uploading API and the image Key used for the image uploading API, and can customize the prompt information when uploading.
5 AppConfig: categorize and add instructions to be more organized.
6 AppMacros: move the Theme Colors configuration item to AppConfig.
7 AppDelegate: add NSUserDefaults configuration item: init once, for something run by App init once.
8 Additional privacy permission description for location always usage has been added.
9 synchronous improved demo App, integrated with AFHTTPTool demo.
10 eggs: continuously click the icon in login to switch server environment, only development/test is valid.

1.4 2019-6-13
AFHTTPTool: configure customizations directly through AFHTTPConfig, optimize the error classification processing.

1.3 2019-5-16
1) New EFUIKit: which adds the ability to directly access the navigation bar based on EFNavigationBar in the controller base class(EFBaseViewController and EFBaseTableViewController). Now you can directly set the gradient background and switch the navigation bar into dark or not (which ACTS on the bar button items on the navigation bar).
2) Demo optimization: code scan is repeatable for more scenarios.
3) Project directory structure optimization, development and organization more balanced.

1.2 2019-2-20
Based on the controller base class encapsulated camera, photo access permission processing methods can now be called independently.
New CodeScanerTool: for scan bar code or QR code.

1.1.2 2018-10-09
Fixed an issue where customized refreshHeader and refreshFooter were not valid after the MJRefreshEnabled wrapped in EFBaseTableViewController was set to YES.

1.1.1 2018-9-20
Optimized demo application. Compatible with Xcode 10, compiled based on the latest SDK.
New Features:
1) EFUtils: DES encryption and decryption related methods, suitable for conventional encryption and decryption.
2) LABiometryTool: iPhone X facial verification.
3) Adapted to apple's policy and improved permission description.

1.1 2018-7-25
Fixed:
1) Fix the problem that no callback is allowed for positioning the second time when positioning is requested in the controller base class.
2) WebTool has fixed the problem that clicking on some special link loading view in WebTool will always show up.
New Features:
1) Demo application.
2) Based on the MJRefresh encapsulated in the table controller base class, simplify the use of MJRefresh encapsulated in the table controller base class. Note that method in a subclass of rewriting (loadData and loadMoreDataWithPageNumber:).
3) The new custom return button integrated in the controller base class not only supports the free combination of navigation buttons, but also customizes methods while maintaining the original gesture return feature.
4) The new custom cancel button integrated in the controller base class not only supports the free combination of navigation buttons, but also customizes methods.

1.0 2017-8-1
Features:
1) controller base class encapsulates a variety of common functions, easy to use.
2) Transparent navigation style is added to the base class of navigation controller.
3) Custom title view and button custom view for navigation in Storyboard.
4) Various common tool components, including interface call, picture upload, local biometric verification, and Web content access. More tool components will be added in the future.
5) Unified configuration items, macros and tool classes for more efficient development.
