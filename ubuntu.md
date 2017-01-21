# Ubuntu 

## 收录架构

i386 x86_64



## 收录版本

12.04 precise

14.04 trusty

16.04 xenial

16.10 yakkety



## 更新频率

每天



## 使用说明

将 `/etc/apt/source.list` 中的地址改为`http://mirror.lzu.edu.cn/ubuntu/` 即可。

或者将该文件替换为以下内容（以 **Ubuntu 16.04 Xenial** 为例，且已默认注释源代码仓库）

```
deb https://mirror.lzu.edu.cn/ubuntu/ xenial main restricted universe multiverse
# deb-src https://mirror.lzu.edu.cn/ubuntu/ xenial main main restricted universe multiverse
deb https://mirror.lzu.edu.cn/ubuntu/ xenial-updates main restricted universe multiverse
# deb-src https://mirror.lzu.edu.cn/ubuntu/ xenial-updates main restricted universe multiverse
deb https://mirror.lzu.edu.cn/ubuntu/ xenial-backports main restricted universe multiverse
# deb-src https://mirror.lzu.edu.cn/ubuntu/ xenial-backports main restricted universe multiverse
deb https://mirror.lzu.edu.cn/ubuntu/ xenial-security main restricted universe multiverse
# deb-src https://mirror.lzu.edu.cn/ubuntu/ xenial-security main restricted universe multiverse
```

修改完成后执行`sudo apt update`或者`sudo apt-get update`