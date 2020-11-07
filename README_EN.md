[中文](README_CN.md)
#Brings Extreme To Development

ExtremeFramework is a complete solution that strives to quickly build the basic framework of iOS project. It is composed of the basic framework of iOS project, the core framework and the core UI. Unified macro and configuration items, a modified global effective, efficient tool method class to solve basic problems, based on the height of the Storyboard encapsulation, automatic layout is the blessing, get rid of the code to customize the worry, highly encapsulation HTTPTool and highly integrated base class method to meet the needs of the common demand instant solutions, integrated toolkit includes integrated payment, fingerprint authentication, common integration functions such as photo upload module.

Hello world! ExtremeFramework！

![Screenshot](http://www.xfmwk.com/images/folders_extreme_framework@2x.png)



## Access Guide

1. Clone from the official git address
2. Modify it to your own project
3. Add your own project files and continue to develop

> * [Quick Start](http://www.xfmwk.com/2019/05/22/快速上手目录/)
> * [Tutorial](http://www.xfmwk.com/categories/开发指南/)
> * [Documents](http://www.xfmwk.com/categories/开发文档/)
> * [FAQ](http://www.xfmwk.com/categories/常见问题/)



## Official Website

Open [Official Website](http://www.xfmwk.com/)



## Release History

### Release

#### 1.5 2019-9-9
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
1. New EFUIKit: which adds the ability to directly access the navigation bar based on EFNavigationBar in the controller base class(EFBaseViewController and EFBaseTableViewController). Now you can directly set the gradient background and switch the navigation bar into dark or not (which ACTS on the bar button items on the navigation bar).
2. Demo optimization: code scan is repeatable for more scenarios.
3. Project directory structure optimization, development and organization more balanced.

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