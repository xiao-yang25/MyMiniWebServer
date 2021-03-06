# MyMiniWebServer

## Linux下最基础的Web服务器。

* 使用**线程池 + 非阻塞socket + epoll(默认LT)** 的并发模型
* 使用**同步IO模拟Proactor** 来进行事件处理
* 使用**状态机**解析HTTP请求报文，默认支持解析GET请求
* 经Webbench压力测试可以实现近五千的并发连接数据交换（虚拟机下实现）

## 压力测试
> * 并发连接总数：4500
> * 访问服务器时间：5s
> * 所有访问均成功

![图片](./resources/images/test.png) 

## 不足
* 定时器
* 日志系统
* CGI校验和连接数据库
