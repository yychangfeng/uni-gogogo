# wit-go

武汉工程大学（WIT）课表 App：登录教务系统导入课表，看本周课表、查成绩、分享课表长图、桌面小组件。

## 📲 下载安装

### 👉 [点这里下载最新版](https://github.com/yychangfeng/wit-go/releases/latest)

打开后点 `wit-go-x.y.z.apk` 下载安装即可。

- 只装 `.apk` 那一个文件。
- `update.json` 是 App 自动检查更新用的，`Source code` 是源码，**都不用管**。
- 首次安装系统会提示，需要允许「安装未知应用」。

## 说明

- 只适配武汉工程大学教务系统（jwxt.wit.edu.cn），使用前需要能访问该系统。
- 数据全部保存在手机本地，不上传服务器；密码可选存在本地用于登录自动填充，App 本身不联网上传任何内容。
- 非官方工具，仅供学习交流，请勿用于商业用途。

## 更新记录

见 [Releases](https://github.com/yychangfeng/wit-go/releases)。

## 🍎 iPhone / 电脑上想看课表？

用浏览器打开 **https://yychangfeng.github.io/wit-go/** ，在 iPhone 的 Safari 里「分享 → 添加到主屏幕」，就是一个全屏的课表 App。

网页版是只读的：数据靠安卓版「导出为文件」生成的 `.json` 导入，**没有上课提醒、没有小组件、没有成绩**（iOS 网页拿不到教务系统页面，也弹不了本地通知）。
