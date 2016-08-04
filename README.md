- ### node-login-register
- #### node编写简易注册登录页面


1. 环境工具

    [nodeJs](www.nodeJs.cn)
    
    检查是否安装成功：node --version
    
    检查npm：npm --version

2. 了解req，res
    
    nodeJs中就是客户端到服务器，产生require请求，然后就是服务器到客户端的回应response。
    在这里我们用到了关键的req.url来判断请求的路径。

3. 读取文件
    
    我们要调用node的包：

    ```
    const http = require('http'); 
    const fs = require('fs');
    ```
    
    我们从***url***里面获得模板路径进行UI渲染。
    
4. 获取数据进行操作

    ```
    var url=urlLib.parse(req.url,true).pathname;
	req.get=urlLib.parse(req.url,true).query;
    ```
    从***urllib***里面获得用户的数据进行注册登录。
