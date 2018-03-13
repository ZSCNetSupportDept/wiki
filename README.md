# [Wiki](http://wiki.sola.love) Repository

## 贡献指南
秉承着[知识属于我们每一个人](https://www.youtube.com/watch?v=eAORm-8b1Eg)的信念，
网络维护科Wiki欢迎每一个人贡献内容。同时，网络维护科感谢为网络维护科Wiki做出过贡献的每一个人。

### 文档格式
所有Wiki页面均使用[Markdown](https://en.wikipedia.org/wiki/Markdown)语言撰写。
你可以通过 *TODO* 了解如何开始上手并撰写Markdown文档。

### 代码仓库
所有Wiki页面的源文件都存放在 [Github 仓库](https://github.com/ZSCNetSupportDept/wiki) 上，
Wiki系统会定时(每5分钟)从Github仓库拉取最新内容并更新。

### 贡献途径
目前，每一个人都可以通过提交 [Pull Request](https://github.com/ZSCNetSupportDept/wiki/pulls) 的方式
向代码仓库提交更改。

你可以 [点击这里](https://github.com/ZSCNetSupportDept/wiki) 了解如何创建 Pull Request。

### 文件名称
系统只会识别 `kebab-case` 的文件，并为其生成Wiki页面。

|文件名|是否识别|
|-----|-------:|
|`foo`|Y|
|`FOO`|N|
|`foo_bar`|N|
|`fooBar`|N|
|`foo-bar`|Y|
