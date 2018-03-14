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

### 系统使用技巧

- 系统五分钟同步一次，若想快速同步，请登录wiki位置，在`设置->系统信息->管理工具->清空缓存和重建索引`处解决

### 文件名称

系统只会识别 `kebab-case` 的文件，并为其生成Wiki页面。

|文件名|是否识别|
|-----|-------:|
|`foo`|Y|
|`FOO`|N|
|`foo_bar`|N|
|`fooBar`|N|
|`foo-bar`|Y|

### 编辑规范

为了便于协作以及维护，请遵循该规范

- 故障页
    - 名称: 故障`故障代码`-`故障名称` eg. `故障651-物理连接错误`
    - 路径: `/article`文件夹
    - 内容要求: 需要有原因及相应的解决方案
- 上传的文件
    - 名称: `故障代码`-`文件名称` eg. `651-overview`
    - 路径: `/uploads`文件夹

### 新建文章

- 使用wiki网站
    1. 点击右上角的 **创建** 按钮
    2. 输入新页面的路径（若为故障页面，推荐 `/article/文件名称`）
    3. 点击创建即可
    4. 更新索引页
- 使用IDE
    1. 在需要的位置新建一个Markdown文件即可
    2. 更新索引页

### 编辑文章

- 使用wiki网站
    1. 打开想要编辑的页面，点击右上角的 **编辑** 按钮
    2. 进行编辑，然后点击右上角的保存即可
- 使用IDE
    1. 打开想要编辑的文件，更改即可
    
### 如何上传文件

- 使用wiki网站
    1. 进入编辑页面
    2. 点击工具栏的 **Insert Image** 或者 **Insert File**按钮
    3. 点击 **上传图片**，选择上传的图片或者文件即可
- 使用IDE
    1. 将文件放进你想放进的文件夹
    
### 如何移动页面

- 使用wiki网站
    1. 进入要移动的页面
    2. 点击右上角 **移动** 按钮
    3. 输入新的路径
    4. 点击 **移动** 即可
    5. 更新索引页
- 使用IDE
    1. 直接更改文件路径即可
    2. 更新索引页
    
### 如何删除页面

- 使用wiki网站
    1. 进入要删除的页面
    2. 点击右上角垃圾桶的图标
    3. 然后点击确定即可
    4. 更新索引页
- 使用IDE
    1. 直接删除文件即可
    2. 更新索引页
    
### 如何找到已创建的页面的URL

- 使用wiki网站
    1. 点击网站左上角的 **所有页面** 按钮
    2. 找到想找的页面
    3. 复制浏览器地址栏的URL
- 使用IDE
    1. 自己算吧233333
    
### 如何创建overview栏

1. 将下面的模版代码，放在 `SUBTITLE` 下，请不要在标签前加空格
    ```text
    <!-- overview: 请将代码放于 SUBTITLE 下 -->
    <div class="overview" style="float:right;border: 1px solid #4054b2;padding:10px;width:280px;background-color: #f9f9fb;margin:10px;">
    <div class="overview-header" style="text-align: center;margin: 5px 0">
    <h3 style="margin:0 0 10px">物理连接错误</h3>
     
    <img src="/uploads/651.png" />
    </div>
    
    <div class="overview-main" style="text-align: left;">
    <div class="overview-item" style="display: grid; grid-template-columns: 100px 1fr;">
    <p style="font-weight: 600;margin: 5px;padding:0;">故障名称</p>
    <p style="margin:5px;padding:0;">物理连接错误</p>
    </div>
    
    <div class="overview-item" style="display: grid; grid-template-columns: 100px 1fr;">
    <p style="font-weight: 600;margin: 5px;padding:0;">故障代码</p>
    <p style="margin:5px;padding:0;">651</p>
    </div>
    
    <div class="overview-item" style="display: grid; grid-template-columns: 100px 1fr;">
    <p style="font-weight: 600;margin: 5px;padding:0;">所属运营商</p>
    <p style="margin:5px;padding:0;">移动、联通</p>
    </div>
    </div>
    </div>
    ```
2. 对代码进行修改即可
