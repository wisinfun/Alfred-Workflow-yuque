# Alfred-Workflow-yuque

👉🏻 **[在MacOS 12.3版本上失效的解决办法](https://lancong.notion.site/Alfred-MacOS-12-3-python-workflow-c97b734dc0954053bb01c754f311bff5)**

搜索个人语雀并获取分享链接

> 此项目是在 https://github.com/xiaotu9639/alfred-yuque-workflow 的基础上完成的
> 
> 新增了快速获取分享链接的功能
> 
> 不支持语雀空间

## ▍使用说明

### 1. 语雀中获取`Token`

头像→账户设置→Token→新建

### 2. 设置`Token`

Alfred中输入`yq > login` ，输入语雀中获取的Token并回车即可

![Untitled](https://user-images.githubusercontent.com/41355260/124374456-e8f97100-dccd-11eb-9a68-79c82e185407.png)


### 3. 设置`Cookie`和`x-csrf-token`

浏览器打开一篇文档，调试模式下可以找到这两个值

![CleanShot 2021-07-04 at 13 15 56@2x](https://user-images.githubusercontent.com/41355260/124374719-4989ad80-dcd0-11eb-8a2c-8c55e2560b60.png)


Alfred全局变量中录入这两个值


![Untitled 2](https://user-images.githubusercontent.com/41355260/124374452-e0089f80-dccd-11eb-9ce3-3a350f292d07.png)


### 4. 使用

- 回车可在浏览器中打开文档（原项目功能）
- 按⌘可将分享链接复制到剪贴板（新增功能）


![Untitled 3](https://user-images.githubusercontent.com/41355260/124374453-e565ea00-dccd-11eb-954c-fa1c20fc200b.png)

