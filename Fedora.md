## Fedora 

## 收录架构

armhfp i386 x86_64



## 收录版本

* Fedora 25
* Fedora 24





## 更新频率

每天



## 使用说明

mirror.lzu.edu.cn 已加入 Fedora 官方镜像列表，一般情况下会根据来源进行自动跳转至最快的镜像。如果您需要手动指定 mirror.lzu.edu.cn 为您的默认源，请**首先备份**`/etc/yum.repos.d/fedora.repo`，然后修改其中的内容为

```
[fedora]
name=Fedora $releasever - $basearch
failovermethod=priority
baseurl=http://mirror.lzu.edu.cn/fedora/releases/$releasever/Everything/$basearch/os/
#metalink=https://mirrors.fedoraproject.org/metalink?repo=fedora-$releasever&arch=$basearch
enabled=1
metadata_expire=7d
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$releasever-$basearch
skip_if_unavailable=False

[fedora-debuginfo]
name=Fedora $releasever - $basearch - Debug
failovermethod=priority
baseurl=http://mirror.lzu.edu.cn/fedora/releases/$releasever/Everything/$basearch/debug/
#metalink=https://mirrors.fedoraproject.org/metalink?repo=fedora-debug-$releasever&arch=$basearch
enabled=0
metadata_expire=7d
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-fedora-$releasever-$basearch
skip_if_unavailable=False
```



修改完成后，执行`sudo dnf makecache`