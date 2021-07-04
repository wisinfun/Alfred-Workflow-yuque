# Alfred-Workflow-yuque

搜索个人语雀并获取分享链接

> 此项目是在 https://github.com/xiaotu9639/alfred-yuque-workflow 的基础上完成的

## ▍使用说明

### 1. 语雀中获取`Token`

头像→账户设置→Token→新建

### 2. 设置`Token`

Alfred中输入`yq > login` ，输入语雀中获取的Token并回车即可

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/262b862f-2c61-4cb6-a240-dc09bf4f170f/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/262b862f-2c61-4cb6-a240-dc09bf4f170f/Untitled.png)

### 3. 设置`Cookie`和`x-csrf-token`

浏览器打开一篇文档，调试模式下可以找到这两个值

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fcbcb0c0-dd75-4914-a39a-18242456d243/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fcbcb0c0-dd75-4914-a39a-18242456d243/Untitled.png)

Alfred全局变量中录入这两个值

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d6051479-378c-44f5-9a16-c8ec6b2ef61d/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d6051479-378c-44f5-9a16-c8ec6b2ef61d/Untitled.png)

### 4. 使用

- 回车可在浏览器中打开文档
- 按⌘可将分享链接复制到剪贴板

![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/eab68e6c-8143-4387-af7b-8837431994cc/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/eab68e6c-8143-4387-af7b-8837431994cc/Untitled.png)
