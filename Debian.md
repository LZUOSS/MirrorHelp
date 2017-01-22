# Debian

## 收录架构

amd64 arm64 armel armhf i386 mips mipsel powerpc ppc64el s390x



## 收录版本

Stable, Old Stable, Testing, Sid



## 更新频率

每天



## 使用说明

一般情况下，将 `/etc/apt/sources.list` 文件备份，并将其中的 Debian 默认的源地址 `http://httpredir.debian.org/` 替换为 `http://mirror.lzu.edu.cn/` 即可。

或者将`/etc/apt/sources.list`的内容替换为（以 **Stable** 版本为例）

```
deb http://mirror.lzu.edu.cn/debian stable main contrib non-free
# deb-src http://mirror.lzu.edu.cn/debian stable main contrib non-free
deb http://mirror.lzu.edu.cn/debian stable-updates main contrib non-free
# deb-src http://mirror.lzu.edu.cn/debian stable-updates main contrib non-free
```

