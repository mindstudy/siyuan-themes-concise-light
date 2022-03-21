# Concise 极简主题



## 特别说明

- 由于隐藏了部分界面元素，本主题需要熟悉思源笔记快捷键，谢谢理解。

## 主题特点

- 优化调整大量细节，界面简明，利于沉浸专注

- 适用于长文档分屏阅读批注等场景

  结合推荐字体，适用于外语学习

思源笔记相关功能介绍：

  [**《思源笔记基本功能详解》**](https://www.yuque.com/u25584857/ryp75p/cd49lz)

  [**《思源笔记双链使用详解》**](https://www.yuque.com/u25584857/ryp75p/tcv57u)

  [**《思源笔记外观修改详解》**](https://www.yuque.com/u25584857/ryp75p/sgf58w)



部分主题效果图：

![行内元素](https://i.imgtg.com/2022/03/20/boeha.png)



![内容块](https://i.imgtg.com/2022/03/20/bo1Es.png)



![文档](https://i.imgtg.com/2022/03/20/boAjN.png)

## 快捷键

本主题由于隐藏了部分界面元素，面板的打开/隐藏需要配合快捷键使用。

一般没打开时，按一次打开，再按一次隐藏。

- 文档树面板 Alt+1 / ⌥1

- 大纲面板 Alt+2 / ⌥2

- 书签面板 Alt+3 / ⌥3

- 标签面板 Alt+4 / ⌥4

- 日记 Alt+5 / ⌥5

- 反链/提及面板 Alt+7 / ⌥7

- 本页关系图面板 Alt+8 / ⌥8

- 全局关系图面板 Alt+9 / ⌥9

- 如果文档树和标签面板同时出现，左边栏关闭按 Alt+4 再按 Alt+，以此类推。

  面板如需改变位置请先切换回默认主题，改变好之后再使用本主题。

## 字体选择

##### 代码字体

- 可使用 Roboto、Noto Sans，效果不错。
- 明色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-light
- 暗色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-dark

##### 图标字体

- 本主题使用图标字体 Font Awesome 6.0.0。

##### 无衬线字体

- 正文标记类文字、除编辑、搜索界面：无衬线字体（黑体）。
- Mac系统自带苹方黑体，显示效果很好。
- Win 系统可在这里下载体验苹方字体：https://uiux.chat/d/63-windows-otf

##### 衬线字体

对于长文档阅读、外语学习，推荐使用衬线字体，辨识度高，缓解长时间使用的视觉疲劳。本主题使用了 Charis SIL、Gentium Plus、方正悠宋、方正准雅宋等衬线字体，需自行安装。不安装界面会显示为无衬线字体（黑体），并不影响使用本主题。

西方语言衬线字体

- 正文英文衬线字体：Charis SIL、Gentium Plus，英文字符、音标、法语、德语、拉丁语、希腊语等显示良好
- Charis SIL、Gentium Plus 的官方网站免费下载（安装其中的regular正体即可，官方提供的粗体斜体Mac系统貌似显示不佳）
- Charis SIL下载 https://software.sil.org/charis/
- Gentium Plus下载 https://software.sil.org/gentium/

中日韩衬线字体

- 方正字体网站以设计师身份注册，可免费个人使用。
- 方正系列字体对中日韩文字的支持很好，但对西文特殊字符支持不佳，故需结合 Charis SIL、Gentium Plus 使用。下载时注意选择GBK版本。
- 正文中文衬线字体：方正悠宋GBK / FZYouSongJ GBK 505L/506L，多个字号建议全装，可选择自己喜欢的字号更改 theme.css 正文字体
- 标题中文衬线字体：方正准雅宋GBK / FZYaSong-M-GBK
- 方正悠宋GBK下载 https://www.foundertype.com/index.php/FontInfo/index/id/5710
- 方正雅宋GBK下载 https://www.foundertype.com/index.php/FontInfo/index/id/193

另外本主题也会用到楷体和仿宋，推荐下载：

- 方正新楷体GBK下载 https://www.foundertype.com/index.php/FontInfo/index/id/290
- 方正仿宋GBK下载 https://www.foundertype.com/index.php/FontInfo/index/id/128

本主题所用字体的字符集涵盖面广，在 Mac 系统下显示良好，其他系统显示效果可能有差异。

字体替换时，字体全称中间如果有空格，css里面需对全称加英文引号。全称除了中文字体名，最好也加上字体的英文名，不然英文系统可能不显示。

可另选自己喜欢的字体修改 theme.css。其他字体参考网站：https://www.qiuziti.com

## 自助修改

如果使用本主题，但对局部不满意，熟悉css的话可以自行修改。

##### 恢复部分隐藏图标

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

##### 恢复笔记本/文档前图标

搜索并删除

```css
/* 隐藏笔记本/文档前图标 */
.b3-list-item__icon{
    display: none !important;
}
```

##### 恢复emoji

本主题隐藏了文档树emoji图标替换面板，如不需要隐藏，请用 EmEditor/Vscode 等文本编辑器打开

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“emoji”，删除下面的语句：

```css
/* 隐藏文档树 emoji 图标修改面板 */
#commonMenu .emojis{
    display: none !important;
}
```

##### 恢复页签关闭按钮

本主题每个页签右侧关闭按钮默认隐藏，鼠标划过该位置时显示。快捷键 Ctrl+w / Cmd+w 关闭更快。

```css
/*文档标题右边关闭按钮*/
.item__close {
    opacity: 10%;
}
.item__close:hover {
    opacity: 88%;
}
```

##### 恢复长文档右侧滚动条

本主题鼠标划过才浮现。由于分屏编辑时页面右侧的滚动条有一定的干扰，本主题在长文档时编辑页面右侧的滚动条默认隐藏，鼠标划过该位置时显示。如需恢复，请删除下面的语句：

```css
/* 长文档滚动条 */
.protyle-scroll.b3-tooltips.b3-tooltips__s{
    opacity: 0;
}
.protyle-scroll.b3-tooltips.b3-tooltips__s:hover{
    opacity: 1;
}
```

##### 恢复删除线

本主题将删除线设置为挖空复习效果，如需恢复，请用 EmEditor/Vscode 等文本编辑器打开对应主题目录的 theme.css，搜索“挖空”，删除下面的语句：

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

##### 恢复镂空/投影

由于行内文字的镂空/投影效果基本不用，本主题将镂空修改为楷体，投影修改为仿宋。由于涉及代码较多，这里就不贴出删除代码。有需要请单独反馈。

## 自定义属性

本主题对内容块可以使用下列自定义属性，方法是在内容块左边的块图标上单击或右键，点击“属性”，然后按“添加”，输入需要的属性名和属性值即可。

| 属性名 | 属性值 | 作用                |
| ------ | ------ | ------------------- |
| f      | bg     | 列表块转换为表格    |
| z      | ht     | 整块/整页转换为黑体 |
| z      | kt     | 整块/整页转换为楷体 |
| z      | fs     | 整块/整页转换为仿宋 |

注意 f - bg 列表块转换为表格功能在左边表格内容较多时会有撑开现象，另外在不同的电脑上浏览器渲染可能不同，会出现部分边线变粗情况，请酌情使用。

## 版本更新

本主题不定期更新，由于主题上传更新有一定时间的等待期，一般 Github 上的仓库会有最新版本，可打包下载，覆盖 Siyuan/conf/appearance/themes/里的同名主题即可。

## 问题反馈

有任何问题，可去 Github Issue 反馈：

https://github.com/mindstudy/siyuan-themes-concise-light/issues

或是语雀相关链接反馈：

https://www.yuque.com/u25584857/ryp75p/zlocwl













