# Concise 极简主题



## 特别提醒

- 本主题隐藏大量界面元素，必须配合思源笔记快捷键使用。

- 不熟悉、不使用思源笔记快捷键的朋友，本主题会很难用，请谨慎下载，谢谢理解。

本主题界面简明，缓解鼠标手，适于沉浸专注，部分效果可参见：

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

- 正文英文衬线字体：Charis SIL、Gentium Plus，英文字符、音标、法语、德语、拉丁语、希腊语等显示良好
- 正文中文衬线字体（除标记类文字）：方正悠宋GBK / FZYouSong GBK 505L/506L，多个字号建议全装，可选择自己喜欢的字号更改 theme.css 正文字体
- 标题中文衬线字体：方正准雅宋GBK / FZYaSong-M-GBK
- 未安装上述衬线字体时，界面显示为无衬线字体（黑体）
- 正文标记类文字、其他界面：无衬线字体（黑体）顺序为苹方、雅黑等
- 明色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-light
- 暗色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-dark

本主题相关字体在 Mac 系统下显示良好。其他系统显示效果可能有差异，可选择自己喜欢的字体做调整。字体网站：https://www.qiuziti.com

## 一些说明

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

### emoji

本主题隐藏了文档树emoji图标替换面板，如不需要隐藏，请用 EmEditor/Vscode 等文本编辑器打开

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“emoji”，删除下面的语句：

```css
/* 隐藏文档树 emoji 图标修改面板 */
#commonMenu .emojis{
    display: none !important;
}
```

### 镂空/投影

由于行内文字的镂空/投影效果基本用不上，本主题将镂空修改为楷体，投影修改为仿宋。由于涉及代码较多，如需恢复，可前往本文档末尾的反馈链接。

### 自定义属性

| 属性名 | 属性值 | 作用                |
| ------ | ------ | ------------------- |
| f      | bg     | 列表块转换为表格    |
| z      | ht     | 整块/整页转换为黑体 |
| z      | kt     | 整块/整页转换为楷体 |
| z      | fs     | 整块/整页转换为仿宋 |

注意 f - bg 列表块转换为表格功能在左边表格内容较多时会有撑开现象，另外在不同的电脑上可以会出现部分边线变粗情况，请酌情使用。

### 鼠标浮现

- 每个页签右侧关闭按钮默认隐藏，鼠标划过该位置时显示。快捷键 Ctrl+w / Cmd+w 关闭更快。
- 由于分屏编辑时页面右侧的滚动条有一定的干扰，本主题在长文档时编辑页面右侧的滚动条默认隐藏，鼠标划过该位置时显示。

### 版本说明

本主题不定期更新，由于主题上传更新有一定时间的等待期，一般 Github 上的仓库会有最新版本，可打包下载，覆盖 Siyuan/conf/appearance/themes/里的同名主题即可。

### 问题反馈

有任何问题，可去 Github Issue 反馈：

https://github.com/mindstudy/siyuan-themes-concise-light/issues

或是语雀相关链接反馈：

https://www.yuque.com/u25584857/ryp75p/zlocwl













