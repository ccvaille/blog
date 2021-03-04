---
title: "我知道的 VSCODE"
date: 2021-03-03T20:24:58+08:00
draft: false
description: "公司内部分享文档"
tags: ["TOOLS"]
---

##### 因为团队内部配置是 Windows，所以介绍是以 Windows 为准。

### 常用命令
- `code -r file`
- `code -d file1 file2`
### 常用操作
- 光标的移动
  - 文件的开头 / 结尾
    - `Ctrl + Home/End`
  - 行首 / 行尾
    - `Home/End`
  - 单词
    - `Alt + →`
    - `Ctrl + →`
  - 代码块
    - `Ctrl + Shift + \`
  - 创建多个光标
    - `Alt + 光标 `
- 文本操作
  - 文本选择
    - 选择左侧 / 右侧的所有内容
      - `Ctrl + Shift + Home/End`
    - 选择单词
      - `Ctrl + Shift + →`
      - 点击两次
    - 整行选择
       - 点击三次鼠标
    - 整个文档选择
      - 点击四次鼠标
    - 选择多行
      - 拖动行号
  - 文本的删除
    - 删除上一个单词
      - `Ctrl + Backspace`
  - 文本的移动
  - 文本的复制(插件)
    - `Ctrl + Shift + D`
    - `alt + ↑`
- 重新打开关闭的编辑页面
  - `Ctrl + shift + T`
- 缩进偏移：左移/右移
  - `Ctrl + [`
  - `Ctrl + ]`
- 打开终端
  - `Ctrl + ` `
- 新建终端
  - `Ctrl + Shift +` `
- 打开命令界面
  - `Ctrl + Shift + P`
- 上一行添加
  - `Ctrl + Shift + Enter`
- 代码折叠/展开
  - `Ctrl + Shift + [`
  - `Ctrl + Shift + ]`
- 搜索
  - 单文件搜索 `Ctrl + F`
  - 多文件搜索 `Ctrl + Shift + F`
- 替换
  - `Ctrl + H`
-  快速分屏
  - `Ctrl + \`
- 快速切换屏
  - `Ctrl + 1`
### 辅助功能
- 鼠标移到函数名上面会显示函数的基本信息，按住 Ctrl 会显示函数的实现
- 鼠标移到 CSS 规则，能看到生效的 HTML 的代码
- 小地图
  - editor.minimap.renderCharacters 渲染每行是实际字符还是色块
- 面包屑
  - breadcrumbs.enabled 开启面包屑
- 空格符
  - editor.renderWhitespace：all 让编辑器将所有的空格符、制表符等全部都渲染出来，可以清楚看出是用空格符还是制表符
- 缩进参考线
  - editor.renderIndentGuides 可以区分出不同代码块之间的层级关系
- 垂直标尺
  - editor.rulers: [150]
- 默认新建语言
  - files.defaultLanguage: 'Markdown'
### 常用命令
- 文件跳转
  - `Ctrl + P`
- 行跳转
  - `:`
  - `Ctrl + G`
- 函数跳转
  - `@`
  - `Ctrl + Shift + O`
### 常用插件
- Chinese (Simplified) Language Pack for Visual Studio Code
- Sublime Text Keymap and Settings Importer
- Vetur
- GitLens — Git supercharged
- Settings Sync
- indent-rainbow
- Todo Tree
- WakaTime
- Polacode-2020
- Import Cost
### 代码块
- 新建
  - 文件-首选项-用户片段
  - `${1:i}`
  - `${1:i}+1`
```JSON
"Print to console": {
		"scope": "javascript,typescript",
		"prefix": "log",
		"body": [
			"console.log('$1');",
			"$2"
		],
		"description": "Log output to console"
	}
```
- [snippet-generator](https://snippet-generator.app/)
#### DEMO
- [HTML-VERSION](/html/我知道的%20VSCODE/index.html)