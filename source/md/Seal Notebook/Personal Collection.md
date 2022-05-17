# Personal Collection



## 价值

[Graham & Doddsville]( https://www.grahamanddoddsville.net/)



## 不错的网站

[李帅奇](https://lishuaiqi.top/tags/)

[蜗窝科技](http://www.wowotech.net/)

[LoyenWang的主页](https://www.cnblogs.com/LoyenWang/)

[Android开发高手课](https://blog.yorek.xyz/android/paid/master/)

[All Android Version ChangeList](https://developer.android.com/about/versions?hl=zh-cn)

[QIANG.LI](https://github.com/lqktz/document)

[Cheson Blog](https://chendongqi.me/)

[生命之旅](https://hazyman.com/)

[Gityuan](http://gityuan.com/)

[颇忒脱的技术博客](https://chanjarster.github.io/)

[Android 性能优化必知必会](https://androidperformance.com/2018/05/07/Android-performance-optimization-skills-and-tools/)

[深入理解Android](https://blog.csdn.net/innost/category_9260827.html)

[老罗的Android之旅](https://blog.csdn.net/luoshengyang?type=blog)

[Android资源大杂烩](https://github.com/coder-pig/Android-Storage-Box/blob/master/Android-Resources-Hodgepodge/Android-Resources-Hodgepodge(Android资源大杂烩).md)

[Android能工巧匠](https://github.com/coder-pig/Android-Storage-Box/blob/master/Android-Skillful-craftsman/Android-Skillful-Craftsman(Android能工巧匠).md)

[Kernel知识点](http://www.ilinuxkernel.com/files/)

[ARNOLDLU](https://github.com/arnoldlu/common-use/tree/master/tools/analyze_suspend)



## Chrome快捷键

[爱上chrome的八个理由之：丰富的快捷键](http://tech.sina.com.cn/s/2011-11-30/08276403237.shtml)

网页后退 Alt + 向左箭头

网页前进 Alt + 向右箭头

重新打开上次关闭的标签页  Ctrl+Shift+T

关闭标签 Ctrl+W

新窗口 Ctrl+N

新的标签页中打开链接 Ctrl+点击

新的Chrome中打开链接 Shift+点击



## Window翻译软件

[QTranslate](https://quest-app.appspot.com/)

[DeepL](https://www.deepl.com/translator)



## Window 文件搜索

[Ererything](https://www.voidtools.com/zh-cn/)



## Python切版本

查看环境变量

```
echo %PATH%
```

所有安装版本查看

```
py -0
```

选取某一个版本执行py

```
py -2.7 C:\Users\seal.wang\Desktop\绩效突破打分工具开发\sourcecode\performance.py
```

依赖库问题解决

```
py -3.7 -m pip install --upgrade pip
py -3.7 -m pip install
```



## Chrome网页截图

1. 右键chrome检查
2. ctrl+shift+p
3. 输入“screenshot”，选择“Capture full size screenshot”



## Notepad++ 模糊搜索

准备以下字符串用来演示 abcdeab cdeabcde abcd eabcde 匹配新行

使用正则表达式

对于 正则表达式的使用方法我们就不介绍了，这里我们搜索abcd字符串。使用下面的正则进行匹配，为了便于显示，我们使用“标记”功能： **a.+?d**

上面的正则表达式的意思是搜索字符串中以a开始，后面有一个或多个字符（.代表除了\n之外的其他字符，+代表匹配一次或多次，?代表非贪婪，即从当前字符开始向后一个一个字符的匹配），最后以d字符结尾。

我们会发现匹配到了4个，可能就会有人问了，那第一行结尾的ab与第二行的cd也应该匹配啊，其实原因就是在于对于正则表达式来说，回车换行代表了一个新的段落开始，如果想匹配那么就涉及到了匹配模式，下面会说明如何进行匹配。

为了解决第3步中我们的问题，在Notepad++中提供了“匹配新行”功能，如果我们选中了，那么就会匹配成功第3步所讲的字符串。



## tree乱码

alias tree='tree --charset ASCII'



##  Window截图

1. 全屏截图 (需要到画图中粘贴)

   Ctrl+PrtScSysRq

2. 选择区域截图

   Win + Shift + S



## Graphviz

https://graphviz.org/download/

使用说明：https://www.jianshu.com/p/6d9bbbbf38b1 

​					https://graphviz.org/doc/info/command.html

dot -Tpng first.dot -o first.png

dot D:\Users\50001806\Desktop\doze.dot -Tsvg -Nfontcolor=red -Nshape=rect > output.svg

建议用法：

dot example.dot -Tsvg -Nfontcolor=red -Nshape=rect -Kcirco > example.svg

dot example.dot -Tpng -Nfontcolor=red -Nshape=rect -Kcirco -o example.png



## Visio的特殊样式

设计-变体（颜色、效果-笔、连接线-笔）



## Visual Studio Code 代码段对齐设置

Perferences-Settings-Editor：Render Indent Guides

vscode显示某文件的所有函数列表
Ctrl+Shift+O  - window

Command+Shift+O -macos

theme：High Contrast



## 100中思维模型

[100种思维模型](https://www.jianshu.com/nb/47934208)



## Q Dir

[Q Dir](http://www.softwareok.com/?Download)



## GitHub

126  美元零九零九大大小

[MAC下访问github速度慢或者无法访问的解决办法](https://zhuanlan.zhihu.com/p/426865721)

[gitpod](https://gitpod.io/workspaces)

[github search docs](https://docs.github.com/cn/search-github/searching-on-github/searching-for-repositories)

[如何在GitHub上搜索](https://blog.csdn.net/u011442726/article/details/100151463)

Github快捷键：

T 键：快速对所有文件进行搜索

L 键：快速跳转到某一行

B 键：快速查看该文件的改动记录

Ctrl+K: 控制面板 



“。”：网页版VScode查看项目

gitpod.io/#/:在线调试



