# future
一个仿照知乎的问答项目,想了很久不知道怎么给这个项目起名,最终还是决定把它当做未来的起点吧!明天会更好!一定!!!

## 项目介绍
利用手头有一套前端页面,然后在百度上找了一个免费网站设计了一下logo.这样,一个曾经理想做一名前端程序员如今对前端已经一窍不通的家伙就开始了他的代码书写,网站的slogan是--`逼乎,和世界分享你刚编的故事`.
为了简化spring数不胜数的配置文件,在这个项目的第一版中使用了springboot进行开发.在这个项目中尽量不写任何配置文件预计在8.23日之前写完,写不完我就是我猪.

## 开发工具
- IDEA+JDK8+git+mysql+springBoot+spring+mybatis


## 项目代码分层介绍

## 实现功能

- 使用拦截器实现了登录与注册功能
- 用前缀树算法实现用户提交文本的敏感词过滤，可有效的对用户提交的非法关键字以及脚本代码进行过滤。
- 使用Redis完成赞和踩以及关注等功能，在高速缓存中的数据存取使得响应速度更加快速。
- 为了能够更快的对用户的请求进行响应，使用生产者消费者模式以及redis实现了一个简单的异步框架。该框架会自动加载实现了EventHandler接口的handler们.并动态选择对应的handler处理请求。
- timeline（新鲜事）功能的实现，向已关注某用户的其他用户推送该用户的最新动态。
- 项目部署,使用ngnix+Tomcat在带宽一兆的服务器上进行的部署,由于加载的js文件过多,所以导致网站速度较为缓慢

## 代码演示
地址: www.indispensable.cn
测试用户账号 user 密码 user
