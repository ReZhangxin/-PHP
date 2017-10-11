# 1.去官网下载php
# 2.测试php是否安装 在`cmd`运行 `php -v`
# 3.进入自己项目的文件夹 在`cmd`中运行 `php -S localhost:0915`
# 4.访问自己的网页 `localhost:0915/admin/admin.php`


## 安装apache不成功
> (OS 10048)通常每个套接字地址(协议/网络地址/端口)只允许使用一次。  : AH00072: make_sock: could not bind to address [::]:443 

> AH00451: no listening sockets available, shutting down 

> AH00015: Unable to open logs 


> 这样的错误是443 端口被占用 

> 解决办法： 

> E:\xampp\apache\conf\extra\httpd-ssl.conf 

> 修改Listen 443 为 Listen 442（这个端口只要没被占用就可使用）

> [xampp配置错误解决方法](http://jingyan.baidu.com/article/ad310e80fbf7fc1848f49e4d.html)

