# 语雀搜索-yuque-Alfred-Workflow

> Uses [alfy](https://github.com/sindresorhus/alfy)
需要 Node.js 14+ 和 [Alfred Powerpack](https://www.alfredapp.com/powerpack/)
> 

## 简介

在 Alfred 中快速搜索语雀文档、浏览器打开文档、复制文档链接、复制文档分享链接

## 功能演示

https://user-images.githubusercontent.com/41355260/182030890-759806c2-da83-4f0b-b6b4-d5e2d3d62461.mp4

- 快速搜索：使用快捷键 `⌃+Y` 或者输入关键词 `yq`，`Enter` 即可在默认浏览器打开文档
- 复制链接：快捷键 `⌘+C`
- 预览文档：快捷键 `⌘+Y`，tips：适用于公开的文档，预览时可以复制文档中的内容
- 拷贝分享链接到剪贴板：快捷键 `⌘+Enter`

## 配置步骤

1. 安装 Node.js
    
    从 [Node 官网](https://nodejs.org/zh-cn/)下载安装，也可以使用 Homebrew 安装
    
    ```bash
    brew install node
    ```
    
2. 在 Release 页下载最新版本 workflow 并安装
3. 在语雀中获取 `Access Token`
    
    打开语雀 → 点击头像 → 账户设置 → Token → 新建 → 授权范围全部勾选并创建 → 复制获取到的 `Access Token` 到Alfred的配置页 `①` 中
    
    ![image](https://user-images.githubusercontent.com/41355260/182030929-8d14553b-1dc9-4b27-a223-74a5e0b93485.png)

    
    ![image](https://user-images.githubusercontent.com/41355260/182030987-6973bb0d-82a3-46ad-9f16-9fdc16fd3ac5.png)

    
    ![image](https://user-images.githubusercontent.com/41355260/182031013-7deabd59-7d2d-4464-adfd-6f8f694be88f.png)

    
4. 从浏览器控制台获取 `cookie` 和 `xToken`（不需要分享功能可跳过）
    
    打开一遍未分享过的文档 → 打开控制台 → 点击页面上的分享按钮并打开分享开关 → 控制台中切换到网络 → 在网络中找到 `share`记录 → 找到 `cookie` 和 `x-csrf-token` → 复制冒号后面的内容到 Alfred 的配置页 `②③` 中
    
    ![image](https://user-images.githubusercontent.com/41355260/182031028-aa619970-701e-4077-8450-45b04da1c4e2.png)

    
    ![image](https://user-images.githubusercontent.com/41355260/182031044-d4d4363c-6762-4311-a695-de52cd822177.png)

