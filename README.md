# weibo
微博架构练习
重构微博系统，基于Servlet/Jsp实现一个简易的MVC框架，具体要求如下：
1、实现3个jsp界面，分别用于注册、登录、微博主页。（对微博的各种操作都在微博主界面中进行，该页面显示微博内容及好友列表，该界面有翻页功能，每页显示最10条微博，最新的显示在最前面；当查看别人的微博时，若不是好友可加好友）
2、所有Http请求格式应为http://xx.xx.xx.xx:8080/blog/YY.do，例如YY可为
Login表示登录微博（缺省，即YY为空时，显示登陆界面）
Reg表示注册
Pub表示发布微博
View表示显示微博
Del表示删除微博
Rep表示回复微博
注意YY.do后面会有?xx1=yy1&xx2=yy2等参数，不做限制
3、浏览器客户端发送http请求能够被MainServlet统一处理,MainServlet为servlet程序，用于控制相关构件处理对微博的各项操作，包括请求URL的映射、调用Modle处理、调用页面显示等。
4、MainServlet要实现统一的URL映射及对Model和View的统一调度，建议用XML定义URL、操作Operation、Model及View之间的映射关系
