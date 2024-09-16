ChatHall
=======
ChatHall forked from walkor/workerman-chat

改名是为了方便区别，侧重点有不同。
基于workerman的GatewayWorker框架开发的一款高性能支持分布式部署的聊天室系统。

GatewayWorker框架文档：http://www.workerman.net/gatewaydoc/


 特性
======
 * 使用websocket协议
 * 多浏览器支持（浏览器支持html5或者flash任意一种即可）
 * 多房间支持
 * 私聊支持
 * 掉线自动重连
 * 微博图片自动解析
 * 聊天内容支持微博表情
 * 支持多服务器部署
 * 业务逻辑全部在一个文件中，快速入门可以参考这个文件[Applications/Chat/Event.php]
  
下载安装
=====
1、git clone https://github.com/beiliwenxiao/ChatHall

2、composer install

启动停止(Linux系统)
=====
以debug方式启动  
```php start.php start  ```

以daemon方式启动  
```php start.php start -d ```

启动(windows系统)
======
双击start_for_win.bat  

注意：  
windows系统下无法使用 stop reload status 等命令  
如果无法打开页面请尝试关闭服务器防火墙  

测试
=======
浏览器访问 http://服务器ip或域:55151,例如http://127.0.0.1:55151

 [更多请访问www.workerman.net](http://www.workerman.net/workerman-chat)

测试例子，仅仅提供从h5直接访问聊天室的例子。
更多的用法一定要看 GatewayWorker框架文档：http://www.workerman.net/gatewaydoc/
通过简单的GatewayWorker的配置，可以很方便的从各类的框架或api的代码中，方便的访问聊天室。

与workerman-chat的区别
=======
新增了一个简单的用户id绑定，方便各类api或mvc框架的用户绑定。


