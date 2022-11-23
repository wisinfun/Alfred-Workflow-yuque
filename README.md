# 语雀搜索-yuque-Alfred-Workflow-使用说明

> Uses [alfy](https://github.com/sindresorhus/alfy) by sindresorhus
  ，需要 Node.js 14+ 和 [Alfred 5 Powerpack](https://www.alfredapp.com/powerpack/)
> 

## 简介

在 Alfred 中快速搜索语雀文档、浏览器打开文档、复制文档链接、切换文档的分享状态

- 快速搜索：打开 Alfred 搜索框，输入 `y + 空格 + 关键词`
- 复制链接：快捷键 `⌘ + C` 或 `Enter`
- 预览文档：快捷键 `⌘ + Y`，tips：适用于公开的文档，预览时可以复制文档中的内容
- 浏览器打开：`⌘ + Enter`
- 浏览器打开并进入编辑模式：`⌘ + ⇧ + Enter`
- 切换文档分享状态：快捷键 `⇧ + Enter`（显示有 🌎 的为已分享状态）

## 配置步骤

1. 安装 Node.js
    
    从 [Node 官网](https://nodejs.org/zh-cn/)下载安装，也可以使用 Homebrew 安装.
    
    ```bash
    brew install node
    ```
    
2. 在 [Release](https://github.com/wisinfun/Alfred-Workflow-yuque/releases) 页下载最新版本 workflow 并安装
3. 在语雀中获取 `Access Token`
    
    打开语雀 → 点击头像 → 账户设置 → Token → 新建 → 授权范围全部勾选并创建 → 复制获取到的 `Access Token` 到Alfred的配置页 ① 中
    
    ![57F1B597-CEE2-4EED-8AC1-887E52762D8D](https://user-images.githubusercontent.com/41355260/202742466-79ac3599-b473-4ff4-8ca4-f4cdf96e3108.png)


    
4. 从浏览器控制台获取 `cookie` 和 `x-csrf-token`（不需要分享功能可跳过）
    
    打开一遍未分享过的文档 → 打开控制台 → 点击页面上的分享按钮并打开分享开关 → 控制台中切换到网络 → 在网络中找到 `meta` 记录 → 找到 `cookie` 和 `x-csrf-token` → 复制冒号后面的内容到Alfred的配置页 ②③ 中
    
    ![786FE528-C884-4D4A-B2A6-A825353BD1A4](https://user-images.githubusercontent.com/41355260/202742479-abca0f19-a42c-4260-9724-f28c89118329.png)


    
5. 配置相关参数
    
    ![7103F5EE-FB79-44F2-A173-9E3BD4A534EF](https://user-images.githubusercontent.com/41355260/202742512-5da138ec-0bed-4069-8d6b-577e91e296e5.png)


