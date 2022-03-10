# Concise 极简主题



## 特别提醒

- 对于不熟悉、不使用思源笔记快捷键的朋友，本主题会很难用，请谨慎下载，谢谢理解。

## 主题特点

- 界面简明，缓解鼠标手，利于沉浸专注
- 适用于长文档分屏阅读批注等场景

部分效果可参见：

  [**《思源笔记基本功能详解》**](https://www.yuque.com/u25584857/ryp75p/cd49lz)

  [**《思源笔记外观修改详解》**](https://www.yuque.com/u25584857/ryp75p/sgf58w)

## 快捷键

### 面板的打开/隐藏

一般没打开时，按一次打开，再按一次隐藏。

- 结构面板（文档树） Alt+1 / ⌥1

- 大纲面板 Alt+2 / ⌥2

- 书签面板 Alt+3 / ⌥3

- 标签面板 Alt+4 / ⌥4

- 日记 Alt+5 / ⌥5

- 反链/提及面板 Alt+7 / ⌥7

- 本页关系面板 Alt+8 / ⌥8

- 全局关系面板 Alt+9 / ⌥9

- 如果文档树和标签面板同时出现，左边栏关闭按 Alt+4 再按 Alt+，以此类推。

  面板如需改变位置请先切换回默认主题，改变好之后再使用本主题。

### 页面切换

- 关闭当前窗口： Ctrl+w / Cmd+w
- 当前窗口前进 Ctrl+] / Cmd+]
- 当前窗口后退 Ctrl+[ / Cmd+[
- 多窗口时向右边窗口切换 Ctrl+Tab / ⌃Tab
- 多窗口时向左边窗口切换 Ctrl+Shift+Tab / ⌃⇧Tab

其他快捷键请参考“设置面板>快捷键”以及官方文档。

## 字体选择

本主题需要安装图标字体 Font Awesome 6.0.0，主题文件夹下font/之中的3个字体安装即可。

对于长文档阅读、外语学习推荐使用衬线字体，缓解长时间使用的视觉疲劳。

- 正文英文衬线字体：Charis SIL、Gentium Plus，英文字符、音标、法语、德语、拉丁语、希腊语等显示良好
- 正文中文衬线字体（除标记类文字）：方正悠宋GBK / FZYouSongJ GBK 505L/506L，多个字号建议全装，可选择自己喜欢的字号更改 theme.css 正文字体
- 标题中文衬线字体：方正准雅宋GBK / FZYaSong-M-GBK

未安装上述衬线字体时，界面显示为无衬线字体（黑体）
- 正文标记类文字、其他界面：无衬线字体（黑体）顺序为苹方、雅黑等
- 明色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-light
- 暗色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-dark

Charis SIL、Gentium Plus 的官方网站免费下载（安装其中的regular正体即可，粗体斜体貌似显示不佳）：

https://software.sil.org/charis/

https://software.sil.org/gentium/

方正字体网站以设计师身份注册，可免费个人使用。

方正系列字体对中日韩文字的支持很好，但对西文特殊字符支持不佳，故需结合 Charis SIL、Gentium Plus 使用。

方正悠宋GBK

https://www.foundertype.com/index.php/FontInfo/index/id/5710

方正雅宋GBK

https://www.foundertype.com/index.php/FontInfo/index/id/193

本主题相关字体在 Mac 系统下显示良好。其他系统显示效果可能有差异，可选择自己喜欢的字体做调整。

字体替换时，字体全称中间如果有空格，css里面需对全称加英文引号。全称最好用字体的英文名，不然其他系统可能显示不正常。

其他字体参考网站：https://www.qiuziti.com

## 一些说明

### 隐藏元素

如果想让某个图标恢复显示，可以搜索一下，找到具体位置，然后删除 `display: none !important;`这一类隐藏语句即可。如果多个图标被一起隐藏，比如下面的css语句，如果想恢复被隐藏的日记图标，就把`#barDailyNote`连同跟在它后面的逗号一起删掉。

```css
/* 日记、同步、主题、多页面前、后切换图标隐藏 */
#barDailyNote,
#barSync,
#barBack,
#barDock,
#barForward {
    display: none !important;
}
```

### emoji

本主题隐藏了文档树emoji图标替换面板，如不需要隐藏，请用 EmEditor/Vscode 等文本编辑器打开

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“emoji”，删除下面的语句：

```css
/* 隐藏文档树 emoji 图标修改面板 */
#commonMenu .emojis{
    display: none !important;
}
```

### 鼠标浮现

每个页签右侧关闭按钮默认隐藏，鼠标划过该位置时显示。快捷键 Ctrl+w / Cmd+w 关闭更快。

```css
/*文档标题右边关闭按钮*/
.item__close {
    opacity: 10%;
}
.item__close:hover {
    opacity: 88%;
}
```

由于分屏编辑时页面右侧的滚动条有一定的干扰，本主题在长文档时编辑页面右侧的滚动条默认隐藏，鼠标划过该位置时显示。如需恢复，请删除下面的语句：

```css
/* 长文档滚动条 */
.protyle-scroll.b3-tooltips.b3-tooltips__s{
    opacity: 0;
}
.protyle-scroll.b3-tooltips.b3-tooltips__s:hover{
    opacity: 1;
}
```

### 挖空

本主题将删除线设置为挖空复习效果，如不需要，请用 EmEditor/Vscode 等文本编辑器打开对应主题目录的 theme.css，搜索“挖空”，删除下面的语句：

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

###镂空/投影

由于行内文字的镂空/投影效果基本用不上，本主题将镂空修改为楷体，投影修改为仿宋。由于涉及代码较多，这里就不贴出删除代码。有需要请单独反馈。

### 自定义属性

| 属性名 | 属性值 | 作用                |
| ------ | ------ | ------------------- |
| f      | bg     | 列表块转换为表格    |
| z      | ht     | 整块/整页转换为黑体 |
| z      | kt     | 整块/整页转换为楷体 |
| z      | fs     | 整块/整页转换为仿宋 |

注意 f - bg 列表块转换为表格功能在左边表格内容较多时会有撑开现象，另外在不同的电脑上可以会出现部分边线变粗情况，请酌情使用。

## 版本说明

本主题不定期更新，由于主题上传更新有一定时间的等待期，一般 Github 上的仓库会有最新版本，可打包下载，覆盖 Siyuan/conf/appearance/themes/里的同名主题即可。

## 问题反馈

有任何问题，可去 Github Issue 反馈：

https://github.com/mindstudy/siyuan-themes-concise-light/issues

或是语雀相关链接反馈：

https://www.yuque.com/u25584857/ryp75p/zlocwl













