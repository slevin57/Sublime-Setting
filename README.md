

# 准备&&说明
## 更改配置文件的路径
Sublime安装完第一次运行的时候，会默认在`%appdata%`目录下生成一个Sublime Text的文件夹，用于存放配置文件及以后安装的各种插件。

我们要做的是不让他在默认的位置生成配置文件，而是要改到我们自定义的软件安装目录中，此时有两种情况：

**情况1**

 Sublime还没安装或者安装之后还没运行过：安装好之后**不要启动**软件，然后进入安装目录，新建一个`Data文件夹`（注意文件夹名称大小写）。
例如我电脑上新建的Data文件夹路径是这样的：`D:\0软件资料包\Sublime Text 3\Data`。

**情况2**

Sublime已经运行过：关掉Sublime，在地址栏输入`%appdata%`进入默认目录，然后删除该目录下的Sublime Text文件夹。不要运行软件，然后按照上面情况1的步骤操作。

经过以上操作再运行软件，所有的配置文件及以后安装的插件就会生成在Data文件夹中了。

## 使用说明
这个仓库存放的是Data目录下Packages文件夹的所有内容，所以如果你准备克隆使用我的插件及配置，先按照上面`更改配置文件的路径`的步骤在软件安装目录创建好Data文件夹，然后进入Data文件夹，克隆这个Repository并命名为`Packages`即可（注意大小写）：

```
git clone <this repository address> Packages
```

执行完上面的步骤，再启动Sublime之后，它就会按照配置文件去自动下载相应的插件。Over。

> 你也可以按如上方式把自己`Packages`文件夹关联到Github上的仓库，这样即使换电脑，只要克隆这个仓库到指定位置就可以快速完成配置了。

# 插件清单（持续更新...）

- Package Control

	Sublime必装，插件管理器。直接去官网，复制对应版本代码到Sublime安装即可。
- HTML-CSS-JS Prettify

	右键格式化html、css、js三种文件类型的代码。
- SublimeTextTrans-master

	调整Sublime的透明度。方法：`视图》Windows Transparency`。

- ZZZZZZZZ-Localization

	经典的Sublime汉化包。安装好之后也可以切换成英文或者别的语言，方法：`帮助》Language`。
- AutoFileName

	自动匹配引入的文件路径。
- Emmet

	不用多说，前端必备，代码自动补全。
- HTML5

	支持HTML5规范的插件包。
- jQuery

	支持jQuery语法。
- JS Snippets

	js语法片段。
- MarkdownEditing

	Markdown语法高亮。
- Sass

	Sass语法文件代码高亮及编译。
- SideBarEnhancements

	可以右键选在直接在浏览器中打开当前文件,l可以设置本地服务器地址及相关打开快捷键。
- SublimeGit

	在Sublime中执行当前目录的Git操作。
- SyncedSideBar

	左边目录树根据当前打开的文件自动定位。
- Vuejs Snippets

	Vue片段自动提示。
- Color Highlighter

	代码表示的颜色以背景或者边框的形式直接显示出来。
- BrackHighlighter

	高亮显示[], (), {}, “”, ”, <tag></tag>符号，便于查看起始和结束标记
- CTags

	Alt+点击函数名称，跳转到相应的函数体。
- Terminal

	打开文件的终端，终端默认是CMD。ctrl+shift+t 打开文件所在文件夹，ctrl+shift+alt+t 打开文件所在项目的根目录文件夹，可以自己重新配置快捷键。也可以Ctrl+Shift+P呼出控制台，输入terminal来选择。
- CSS Format

	将任意的 CSS、SASS、SCSS、LESS 代码格式化为展开、紧凑、压缩的形式，选中需要格式化的样式代码，右键选中CSS Format，选择需要形成的格式即可。
	
- Word Count

	在左下角显示当前文件的单词数量。

# 自定义配置（持续更新...）
- 全部保存快捷键设置

	在用户的快捷键设置中，输入:
	
	```[
	{ "keys": ["ctrl+shift+s"], "command": "save_all" }
	]```