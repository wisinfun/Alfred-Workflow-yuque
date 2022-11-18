# 语雀搜索-yuque-Alfred-Workflow-使用说明-1.4

> Uses [alfy](https://github.com/sindresorhus/alfy) by sindresorhus
需要 Node.js 14+ 和 [Alfred 5 Powerpack](https://www.alfredapp.com/powerpack/)
> 

## 简介

在 Alfred 中快速搜索语雀文档、浏览器打开文档、复制文档链接、切换文档的分享状态

- 快速搜索：使用快捷键 `⌃+Y` 或者输入关键词 `yq`，`Enter`
即可在默认浏览器打开文档
- 复制链接：快捷键 `⌘+C` 或 `⌘+Enter`
- 预览文档：快捷键 `⌘+Y`，tips：适用于公开的文档，预览时可以复制文档中的内容
- 切换文档分享状态：快捷键 `⇧+Enter`

## 配置步骤

1. 安装 Node.js
    
    从 [Node 官网](https://nodejs.org/zh-cn/)下载安装，也可以使用 Homebrew 安装
    
    ```bash
    brew install node
    ```
    
2. 在 [Release](https://github.com/wisinfun/Alfred-Workflow-yuque/releases) 页下载最新版本 workflow 并安装
3. 在语雀中获取 `Access Token`
    
    打开语雀 → 点击头像 → 账户设置 → Token → 新建 → 授权范围全部勾选并创建 → 复制获取到的 `Access Token` 到Alfred的配置页 ① 中
    
    https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fc87de44a-3cb4-4c72-9dd7-3f1551e04b9f%2FUntitled.png?table=block&id=4507b05b-618e-4cc5-b18a-ca0519c02a57&spaceId=b4796fe7-20d9-4113-be6a-34e95c3067b7&width=2000&userId=8037e86d-0da3-4ba5-b1b0-ad106e290957&cache=v2![image](https://user-images.githubusercontent.com/41355260/202741957-411b7292-29b8-41a4-83b1-45944f8936e7.png)

    
4. 从浏览器控制台获取 `cookie` 和 `x-csrf-token`（不需要分享功能可跳过）
    
    打开一遍未分享过的文档 → 打开控制台 → 点击页面上的分享按钮并打开分享开关 → 控制台中切换到网络 → 在网络中找到 `meta` 记录 → 找到 `cookie` 和 `x-csrf-token` → 复制冒号后面的内容到Alfred的配置页 ②③ 中
    
    https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Faf523db9-7875-4a28-9d08-965dd15fad14%2FUntitled.png?table=block&id=a8e69fee-180b-45d6-800b-1dd56a824613&spaceId=b4796fe7-20d9-4113-be6a-34e95c3067b7&width=2000&userId=8037e86d-0da3-4ba5-b1b0-ad106e290957&cache=v2![image](https://user-images.githubusercontent.com/41355260/202742020-b8a1d8f2-5c86-45d4-bb46-9584e54dcd83.png)

    
5. 配置相关参数
    
    https://www.notion.so/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2F12e1662e-ec24-4b68-8da1-8aa01f9a4b2d%2FUntitled.png?table=block&id=a96fe58f-d616-4c32-8879-6b677f86892d&spaceId=b4796fe7-20d9-4113-be6a-34e95c3067b7&width=2000&userId=8037e86d-0da3-4ba5-b1b0-ad106e290957&cache=v2![image](https://user-images.githubusercontent.com/41355260/202742067-82bfbc69-034d-48fc-bdfd-228de36c926b.png)

