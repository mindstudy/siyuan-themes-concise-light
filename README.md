# Concise 极简主题

## 介绍

主题部分效果可参见：

[**《思源笔记基本功能详解》**](https://www.yuque.com/u25584857/ryp75p/cd49lz)

[**《思源笔记外观修改详解》**](https://www.yuque.com/u25584857/ryp75p/sgf58w)



## 特点

* 隐藏一些界面元素，并优化细节
* 配合快捷键使用，缓解鼠标手
* 界面简明，适于沉浸专注

## 字体

正文英文衬线字体：Charis SIL，英文字符、音标显示较好

正文中文衬线字体（除标记类文字）：方正悠宋GBK / FZYouSong GBK（多个字号建议全装）

标题中文衬线字体：方正准雅宋GBK / FZYaSong-M-GBK

未安装上述衬线字体时，界面显示为无衬线字体（黑体）

正文标记类文字、其他界面：无衬线字体（黑体）顺序为苹方、雅黑等



明色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-light。

暗色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-dark。

字体网站：https://www.qiuziti.com

## 说明

### 挖空

本主题将删除线设置为挖空复习效果，如不需要，请用 EmEditor/Vscode 等文本编辑器打开。

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“挖空”，删除下面的语句：

```css
.protyle-wysiwyg s{
    color: transparent;
    border-bottom: 1px solid #555;
    transition: color 0.2s ease-in-out !important;
    text-decoration: none;
}

.protyle-wysiwyg [data-node-id] [spellcheck="false"] s:hover{
    color: #333;
    background-color: transparent;
    text-decoration: none;
    border-bottom:  none;
```

### emoji

本主题隐藏了文档树emoji图标替换面板，如不需要，请用 EmEditor/Vscode 等文本编辑器打开

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“emoji”，删除下面的语句：

```css
/* 隐藏文档树 emoji 图标修改面板 */
#commonMenu .emojis{
    display: none !important;
}
```

### 镂空/投影

本主题将镂空修改为楷体，投影修改为仿宋。

### 自定义属性

| 属性名 | 属性值 | 作用                |
| ------ | ------ | ------------------- |
| f      | bg     | 列表块转换为表格    |
| z      | kt     | 整块/整页转换为楷体 |
| z      | fs     | 整块/整页转换为仿宋 |

注意列表块转换为表格功能在左边表格内容较多时会有撑开现象，另外在不同的电脑上可以会出现边线变粗情况，请酌情使用。

## 快捷键

本主题需配合快捷键使用，降低鼠标手疲劳。

### 页面切换

关闭当前窗口： Ctrl+w / Cmd+w

窗口页面内容跳转多次时：

当前窗口前进 Ctrl+] / Cmd+]

当前窗口后退 Ctrl+[ / Cmd+[

多窗口时向右边窗口切换 Ctrl+Tab / ⌃Tab

多窗口时向左边窗口切换 Ctrl+Shift+Tab / ⌃⇧Tab

### 面板的打开/隐藏

按一次打开，按两次显示。

结构面板（文档树） Alt+1 / ⌥1

大纲面板 Alt+2 / ⌥2

书签面板 Alt+3 / ⌥3

标签面板 Alt+4 / ⌥4

日记 Alt+5 / ⌥5

反链/提及面板 Alt+7 / ⌥7

本页关系面板 Alt+8 / ⌥8

全局关系面板 Alt+9 / ⌥9



如果文档树和标签面板同时出现，左边栏关闭按 Alt+4 再按 Alt+，以此类推。

其他快捷键请参考“设置面板>快捷键”以及官方文档。



有任何问题，可去 Github Issue、语雀相关链接反馈。













