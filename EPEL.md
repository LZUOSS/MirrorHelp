# EPEL

Extra Packages for Enterprise Linux

## 收录架构

armhfp i386 x86_64



## 收录版本

    EPEL 7: x86_64, ppc64, ppc64le, aarch64, sources
    EPEL 6: i386, x86_64, ppc64, sources
    EPEL 5: i386, x86_64, ppc, sources 


## 更新频率

每天



## 使用说明

mirror.lzu.edu.cn 已加入 EPEL 官方镜像列表，一般情况下会根据来源进行自动跳转至最快的镜像。如果您需要手动指定 mirror.lzu.edu.cn 为您的默认源，请**首先备份**`/etc/yum.repos.d/epel.repo`以及`/etc/yum.repos.d/epel-testing.repo`，然后根据不同版本修改其中的内容为

### CentOS 7 / RHEL 7

`/etc/yum.repos.d/epel.repo`

```
[epel]
name=Extra Packages for Enterprise Linux 7 - $basearch
baseurl=http://mirror.lzu.edu.cn/epel/7/$basearch
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-7&arch=$basearch
failovermethod=priority
enabled=1
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
 
[epel-debuginfo]
name=Extra Packages for Enterprise Linux 7 - $basearch - Debug
baseurl=http://mirror.lzu.edu.cn/epel/7/$basearch/debug
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-debug-7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1
 
[epel-source]
name=Extra Packages for Enterprise Linux 7 - $basearch - Source
baseurl=http://mirror.lzu.edu.cn/epel/7/SRPMS
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-source-7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1
```

`/etc/yum.repos.d/epel-testing.repo`

```
[epel-testing]
name=Extra Packages for Enterprise Linux 7 - Testing - $basearch
baseurl=http://mirror.lzu.edu.cn/epel/testing/7/$basearch
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-epel7&arch=$basearch
failovermethod=priority
enabled=0
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
 
[epel-testing-debuginfo]
name=Extra Packages for Enterprise Linux 7 - Testing - $basearch - Debug
baseurl=http://mirror.lzu.edu.cn/epel/testing/7/$basearch/debug
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-debug-epel7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1
 
[epel-testing-source]
name=Extra Packages for Enterprise Linux 7 - Testing - $basearch - Source
baseurl=http://mirror.lzu.edu.cn/epel/testing/7/SRPMS
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-source-epel7&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-7
gpgcheck=1
```

### CentOS 6 / RHEL 6

`/etc/yum.repos.d/epel.repo`

```
[epel]
name=Extra Packages for Enterprise Linux 6 - $basearch
baseurl=http://mirror.lzu.edu.cn/epel/6/$basearch
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-6&arch=$basearch
failovermethod=priority
enabled=1
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
 
[epel-debuginfo]
name=Extra Packages for Enterprise Linux 6 - $basearch - Debug
baseurl=http://mirror.lzu.edu.cn/epel/6/$basearch/debug
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-debug-6&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
gpgcheck=1
 
[epel-source]
name=Extra Packages for Enterprise Linux 6 - $basearch - Source
baseurl=http://mirror.lzu.edu.cn/epel/6/SRPMS
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=epel-source-6&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
gpgcheck=1
```

`/etc/yum.repos.d/epel-testing.repo`

```
[epel-testing]
name=Extra Packages for Enterprise Linux 6 - Testing - $basearch
baseurl=http://mirror.lzu.edu.cn/epel/testing/6/$basearch
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-epel6&arch=$basearch
failovermethod=priority
enabled=0
gpgcheck=1
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
 
[epel-testing-debuginfo]
name=Extra Packages for Enterprise Linux 6 - Testing - $basearch - Debug
baseurl=http://mirror.lzu.edu.cn/epel/testing/6/$basearch/debug
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-debug-epel6&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
gpgcheck=1
 
[epel-testing-source]
name=Extra Packages for Enterprise Linux 6 - Testing - $basearch - Source
baseurl=http://mirror.lzu.edu.cn/epel/testing/6/SRPMS
#mirrorlist=https://mirrors.fedoraproject.org/metalink?repo=testing-source-epel6&arch=$basearch
failovermethod=priority
enabled=0
gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-EPEL-6
gpgcheck=1
```


修改完成后，执行`sudo yum makecache` 