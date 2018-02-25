# 准备工作
首先判断是否通过客户端进行终端连接
打开Xshell 尝试连接服务器，如果出现 访问连接失败 提示22端口未打开
那么从云服务器控制台进入。

```
ss -lnt

```
 是否有22端口打开
![image.png](/.attachments/image-597aef9d-6f8a-460e-8189-3ac215be7160.png)

如果没有的话，执行
```


service sshd restart

```
打开端口。

