# 安装Docker 

- 首先我们更新下APT软件包的源

`
$ sudo apt-get update  
`
- 安装软件包以允许apt通过HTTPS使用存储库

```

$ sudo apt-get install \
apt-transport-https \
ca-certificates \
curl \
software-properties-common
```

> 因为国内特色，所以以下提供的官方镜像，恩恩。我们替换为教育网的镜像。

 - 添加Docker的官方GPGkey 
 
## 官方：
```
$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add 
```

## 教育网：

```
$ curl -fsSL https://mirrors.ustc.edu.cn/docker-ce/linux/ubuntu/gpg | sudo apt-key add 
```


- 进行密钥的匹配

```
$ sudo apt-key fingerprint 0EBFCD88
pub   4096R/0EBFCD88 2017-02-22
      Key fingerprint = 9DC8 5822 9FC7 DD38 854A  E2D8 8D81 803C 0EBF CD88
uid                  Docker Release (CE deb) <docker@docker.com>
sub   4096R/F273FCD8 2017-02-22
```


- 我们需要向  source.list  中添加 Docker 软件源

## 官方：

```
$ sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"
   
   ```

## 教育网

```
$ sudo add-apt-repository \
"deb [arch=amd64] https://mirrors.ustc.edu.cn/docker-ce/linux/ubuntu \
$(lsb_release -cs) \
stable"

```

## 安装Docker

 - 更新下我们的软件源

   ```
    $  sudo apt-get update
    ```
- 安装最新版本的Docker CE

```
   $ sudo apt-get install docker-ce
```

> 安装制定版本的docker

```
$ sudo apt-get install docker-ce=<VERSION>

列出版本

apt-cache policy docker-ce

>  17.12.0~ce-0~ubuntu  
sudo apt-get install docker-ce=17.12.0~ce-0~ubuntu  
```
 
 
 # 启动 Docker
 
配置Docker自启动，
```
 $ sudo systemctl enable docker
```
> 要禁用此行为，请disable改为使用。
```
$ sudo systemctl disable docker
```
**启动Docker**
```
$ sudo systemctl start docker
```
 
### 将当前登陆用户添加到Docker用户组

建立  docker  组：

```
$ sudo groupadd docker
```

将当前用户加入  docker  组：

```
$ sudo usermod -aG docker $USER
```

退出当前终端并重新登录，进行如下测试。 
 
 ```
 $ docker run hello-world
 ```
 
 
 
 
 ## ===分割线===
 
 # 卸载 Docker CE
 - 卸载Docker CE
```
$ sudo apt-get purge docker-ce
```
主机上的图像，容器，卷或自定义配置文件不会自动删除。此命令是删除所有图像，容器和卷：
```
$ sudo rm -rf /var/lib/docker
 ```
 
 
 
 
 
 
