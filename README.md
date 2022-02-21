# Concise 极简主题

## 介绍

[**《思源笔记基本功能详解》**](https://www.yuque.com/u25584857/ryp75p/cd49lz)

[**《思源笔记外观修改详解》**](https://www.yuque.com/u25584857/ryp75p/sgf58w)



## 特点

* 隐藏一些界面元素，并优化细节

* 配合快捷键使用，缓解鼠标手

  界面简明，适于沉浸专注

明色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-light。

暗色主题配套代码块主题，推荐在设置>代码块主题选择 atom-one-dark。



![preview](preview.png)



新版主题将删除线设置为挖空复习效果，如不需要，请用 EmEditor/Vscode 等文本编辑器打开

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“挖空”，删除下面的语句：

```css
/* 修改高亮为挖空效果*/
.protyle-wysiwyg mark{
    color: transparent;
    transition: color 0.2s ease-in-out;
}
.protyle-wysiwyg [data-node-id] [spellcheck="false"] mark:hover{
    color: var(--b3-protyle-inline-mark-color);
    background-color: transparent;
} /* 挖空效果*/
```

本主题隐藏了文档树emoji图标替换面板，如不需要，请用 EmEditor/Vscode 等文本编辑器打开

Siyuan/conf/appearance/themes/Concise Lght/theme.css，搜索“emoji”，删除下面的语句：

```css
/* 隐藏文档树 emoji 图标修改面板 */
#commonMenu .emojis{
    display: none !important;
}
```



## 快捷键

### 页面切换

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













