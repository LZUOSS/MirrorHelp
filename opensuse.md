# OpenSUSE

## 收录架构

i586 x86_64

## 收录版本

12.1

12.2

12.3

13.1

Leap 42.1

Leap 42.2

## 更新频率

//

## 使用说明

禁用所有原有的软件源
`sudo zypper mr -da`

添加兰大软件源（以 openSUSE Leap 42.2 为例，源的别名为 LZUOSS-XXX）
`sudo zypper ar -fc http://mirror.lzu.edu.cn/opensuse/distribution/leap/42.2/repo/oss/ LZUOSS-OSS`
`sudo zypper ar -fc http://mirror.lzu.edu.cn/opensuse/distribution/leap/42.2/repo/non-oss LZUOSS-NON-OSS`
`sudo zypper ar -fc http://mirror.lzu.edu.cn/opensuse/update/leap/42.2/oss LZUOSS-UPDATE-OSS`
`sudo zypper ar -fc http://mirror.lzu.edu.cn/opensuse/update/leap/42.2/non-oss LZUOSS-UPDATE-NON-OSS`

刷新软件源
`sudo zypper ref`