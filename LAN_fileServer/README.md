# LAN_fileServer
这是一个十分简单的基于Flask和Python2.7.12的局域网文件服务器

需要配合着Nginx服务器发送文件。

Flask代码部分的主要功能：

​	从资源文件夹中获取文件的路径，将路径转换为URL返回给前端页面

Nginx部分主要功能：

​	核心：做静态文件处理

​	提供前端网页「文件列表页面」，

​	根据前端的请求将文件列表中的文件发送前端

​	将前端对文件列表中所有文件的URL的请求转发给Flask服务

前端页面部分：

​	核心：展示文件列表	

​	通过ajax向后端发送获取所有文件URL的请求并渲染到页面上