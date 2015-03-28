Learning Sublime Text (系统学习ST)
=======================

编辑、整理 By Xujiajun
- - -
前言
----
如何编辑本文？[请点击这里](https://github.com/xujiajun/Learning-Sublime-Text/edit/master/README.md)

如何fork本文？点击右上角"Fork" 按钮.

如何发pull Requests 作出贡献? [请点击这里] (https://github.com/xujiajun/Learning-Sublime-Text/pulls)

1、Why Sublime Text?
----
 0、高效（启动快、快键键强大）

 1、扩展性强（插件丰富）

 2、主题丰富
 
 3、支持多屏、多变量操作
 
 4、跨平台
 
 5、不注册亦可免费使用（ 有米的童靴可以支持下原作者 [USD $70](https://www.sublimetext.com/buy) ）
 
 6、支持自定义

2、Sublime Text 安装以及简介
------
 Sublime Text 2 下载地址：[http://www.sublimetext.com/2]
 
 Sublime Text 3 下载地址：[http://www.sublimetext.com/3] [推荐]

3、主题
------
 安装Colorsublime-Plugin来扩展主题
 
 0、打开ST的命令面板  ctl+shift+p (Windows/Linux) or ⇧+⌘+p (OSX)
 
 1、选择Colorsublime: Install Theme
 
 2、用箭头键来浏览各个主题、你可以实时看到切换的主题变化！
 
 [Colorsublime官网](http://colorsublime.com/)
 
4、常用命令
--------
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

5、命令行工具
-----------------------
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

6、自定义配置
------------------------
7、Package Control安装以及使用
-------------------------
8、插件安装以及使用
-------------------------
9、定制代码片段
--------------------------
