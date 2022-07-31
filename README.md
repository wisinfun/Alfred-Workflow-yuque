# 语雀搜索-yuque-Alfred-Workflow

> Uses [alfy](https://github.com/sindresorhus/alfy)
需要 Node.js 14+ 和 [Alfred Powerpack](https://www.alfredapp.com/powerpack/)
> 

## 简介

在 Alfred 中快速搜索语雀文档、浏览器打开文档、复制文档链接、复制文档分享链接

## 功能演示

[Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7e0116a8-807e-4e23-a625-d6a0bee62e9a/Untitled.mp4)

- 快速搜索：使用快捷键 `⌃+Y`或者输入关键词`yq`
- 复制链接：快捷键`⌘+C`
- 预览文档：快捷键`⌘+Y`，tips：适用于公开的文档，预览时可以复制文档中的内容
- 拷贝分享链接到剪贴板：快捷键`⌘+Enter`

## 配置步骤

1. 安装 Node.js
    
    从 [Node 官网](https://nodejs.org/zh-cn/)下载安装，也可以使用 Homebrew 安装
    
    ```bash
    brew install node
    ```
    
2. 在 Release 页下载最新版本 workflow 并安装
3. 在语雀中获取 `Access Token`
    
    打开语雀 → 点击头像 → 账户设置 → Token → 新建 →授权范围全部勾选并创建 → 复制获取到的 `Access Token` 到Alfred的配置页①中
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c87de44a-3cb4-4c72-9dd7-3f1551e04b9f/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/13760ffa-41ae-4412-bb59-c500c26f1cac/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5079fb96-f8d6-4a65-b4cc-94a2ea23f5b1/Untitled.png)
    
4. 从浏览器控制台获取 `cookie` 和 `xToken`（不需要分享功能可跳过）
    
    打开一遍未分享过的文档 → 打开控制台 → 点击页面上的分享按钮并打开分享开关 → 控制台中切换到网络 → 在网络中找到 `share`记录 →找到 `cookie` 和 `x-csrf-token` →复制冒号后面的内容到Alfred的配置页②③中
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1b850da0-0b54-42a8-8f74-31841d4a7baa/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5079fb96-f8d6-4a65-b4cc-94a2ea23f5b1/Untitled.png)
