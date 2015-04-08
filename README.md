Learning Sublime Text (系统学习ST)
=======================

编辑、整理 By Xujiajun
- - -
前言
----
如何编辑本文？[请点击这里](https://github.com/xujiajun/Learning-Sublime-Text/edit/master/README.md)

如何fork本文？点击右上角"Fork" 按钮.

如何发pull Requests 作出贡献? [请点击这里] (https://github.com/xujiajun/Learning-Sublime-Text/pulls)

目录导航
---
- [1、Why Sublime Text?](#why-st)
- [2、Sublime Text 安装以及简介](#st-install)
- [3、主题](#st-theme)
- [4、常用命令](#st-command)
- [5、命令行工具](#st-command-tool)
- [6、自定义配置](#st-preference)
- [7、Package Control安装以及管理](#st-pc-install)
- [8、插件安装以及使用](#st-plugin-install)
- [9、定制代码片段](#st-snippet)

<h2 id="why-st">1、Why Sublime Text?</h2>

 0、高效（启动快、快键键强大）

 1、扩展性强（插件丰富）

 2、主题丰富
 
 3、支持多屏、多变量操作
 
 4、跨平台
 
 5、不注册亦可免费使用（ 有米的童靴可以支持下原作者 [USD $70](https://www.sublimetext.com/buy) ）
 
 6、支持自定义
 
<b>更多介绍，请观看视频</b>：http://superu.org/course/2/learn#lesson/3
<h2 id="st-install">2、Sublime Text 安装以及简介</h2>

Sublime Text 2 下载地址：[http://www.sublimetext.com/2]
 
Sublime Text 3 下载地址：[http://www.sublimetext.com/3] [推荐]

<b>更多介绍，请观看视频</b>: http://superu.org/course/2/learn#lesson/8
<h2 id="st-theme">3、主题</h2>

 安装Colorsublime-Plugin来扩展主题
 
 0、打开ST的命令面板  ctl+shift+p (Windows/Linux) or ⇧+⌘+p (OSX)
 
 1、选择Colorsublime: Install Theme
 
 2、用箭头键来浏览各个主题、你可以实时看到切换的主题变化！
 
 [Colorsublime官网](http://colorsublime.com/)
 
<h2 id="st-command">4、常用命令</h2>

<table>
  <tr>
     <td>cmd+p (cmd+t)</td>
     <td>文件、行数、函数定位</td>
  </tr>
<tr>
	<td>cmd+d</td>
	<td>多选</td>
</tr>
<tr>
	<td>cmd+r</td>
	<td>函数定位</td>
</tr>
<tr>
	<td>ctrl+g</td>
	<td>行数定位</td>
</tr>
<tr>
    <td>cmd+]/[ (shift+tab)</td>
    <td>行缩进</td>
</tr>
<tr>
    <td>cmd+shift+v</td>
    <td>复制[带格式化]</td>
</tr>

<tr>
    <td>cmd+shift+t</td>
    <td>回退</td>
</tr>

<tr>
    <td>cmd+control+⬆/⬇</td>
    <td>行上下移动</td>
</tr>
 <tr>
     <td>cmd+shift+d </td>
     <td>复制光标当前行</td>
 </tr>
 <tr>
     <td>cmd+X(shift+control+k)</td>
     <td>删除光标当前行</td>
 </tr>
 <tr>
   <td>cmd + f </td>
   <td>查找当前文件</td>
 </tr>
 <tr>
    <td>cmd + option + 2</td>
    <td>把屏幕分成2份  （其他同理）</td>
 </tr>
 <tr>
    <td>cmd + k + b</td>
    <td>开关边侧栏</td>
 </tr>
</table>

<h2 id="st-command-tool">5、命令行工具</h2>

sudo ln -s "/Applications/Sublime Text.app/Contents/SharedSupport/bin/subl" /usr/bin/subl

**用法**

	运行 subl --help
	Usage: subl [arguments] [files]         编辑指定的文件edit the given files
	   or: subl [arguments] [directories]   打开指定的目录
	   or: subl [arguments] -               编辑stdin
	
	 Arguments:
	  --project <project>: 载入指定的project
	  --command <command>: 运行指定的命令
	  -n or --new-window:  打开一个新的窗口
	  -a or --add:         添加文件夹到当前窗口
	  -w or --wait:        返回前等待文件关闭
	  -b or --background:  不激活该应用程序
	  -s or --stay:        文件关闭后保持应用程序激活状态
	  -h or --help:        显示帮助并退出
	  -v or --version:     显示版本信息并退出
    
 如果从标准输入--wait是隐式的。 使用--stay当文件关闭是不切换到后台控制台(只与是否有等待的文件有关)。

 文件名可以通过加:line或者:line:column后缀来指定打开的定位。
 
 更多介绍，请观看视频：http://superu.org/course/2/learn#lesson/9
<h2 id="st-preference">6、自定义配置</h2>

	{
		"color_scheme": "Packages/Colorsublime - Themes/Monokai.tmTheme",
		"create_window_at_startup": false,
		"font_size": 15,
		"highlight_line": true,
		"highlight_modified_tabs": true,
		"ignored_packages":
		[
			"Vintage",
			"Markdown"
		],
		"show_debug": true,
		"show_encoding": true,
		"show_full_path": true,
		"translate_tabs_to_spaces": true
	}

<h2 id="st-pc-install">7、Package Control安装以及使用</h2>

mac下opt+` 或者 菜单栏选择View > Show Console
	
>ST3:

	import urllib.request,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by)


>ST2:

	import urllib2,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')

<h2 id="st-plugin-install">8、插件安装以及使用</h2>

0、shift + cmd + p 打开命令面板

1、输入 “Package Control: Install Package” 命令或者install 关键词找到 “Package Control: Install Package”

2、输入安装插件的简写或全拼,找到后回车安装

<h2 id="st-snippet">9、定制代码片段</h2>

在编写代码的时候，有遇到反复使用的代码片段，这时候就需要复制、黏贴，大大影响效率。我们利用Sublime Text的snippet功能,就能很好的解决这一问题.

如何创建？Tools > New Snippet
会出现如下：

	<snippet>
	    <content><![CDATA[
	Hello, ${1:this} is a ${2:snippet}.
	]]></content>
	    <!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	    <!-- <tabTrigger>hello</tabTrigger> -->
	    <!-- Optional: Set a scope to limit where the snippet will trigger -->
	    <!-- <scope>source.python</scope> -->
	</snippet>

看不懂？ok我们看下例子

创建我的第一个Snippet：

	<snippet>
	    <content><![CDATA[ 你需要插入的代码片段${1:name} ]]></content>
	    <!-- 可选：快捷键，利用Tab自动补全代码的功能,这里你输入superu即可触发 -->
	    <tabTrigger>superu</tabTrigger>
	    <!-- 可选：使用范围，不填写代表对所有文件有效。 -->
	    <scope>source.python</scope>
	    <!-- 可选：在snippet菜单中的显示说明（支持中文）。如果不定义，菜单则显示当前文件的文件名。 -->
	    <description>My first Snippet</description>
	</snippet>

${1:name}表示代码插入后，光标所停留的位置，可同时插入多个。其中:name为自定义参数（可选）。

${2}表示代码插入后，按Tab键，光标会根据顺序跳转到相应位置（以此类推）。

