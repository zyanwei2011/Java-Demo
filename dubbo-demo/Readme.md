### 介绍
+ 001+002:    为生产者+消费者直连模式
+ 003+004+005:    将接口项目独立出来，为dubbo官方推荐模式
+ 006+007+008:    将接口项目独立出来，并配置zookeeper
### zk方式访问
+ wen访问
>url: http://127.0.0.1:8080/userDetail?id=2323&username=lllls

+ telnet访问
```shell
$ telnet 127.0.0.1 20880
Trying 127.0.0.1...
Connected to localhost.
Escape character is '^]'.

dubbo>invoke com.bjpowernode.dubbo.service.UserService.queryUserById(1223,"lili")  
{"id":1223,"username":"2lili"}
```
