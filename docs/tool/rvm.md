---
layout: default
title: Ruby版本管理工具rvm
parent: tool
---
----
## rvm 安装
```shell{.line-numbers}
curl -l get.rvm.io | bash -s stable
source ~/.bashrc
source ~/.bash_profile
```

## 修改 rvm 的 ruby 安装源到国内的淘宝镜像服务器
```
sed -i -e 's/ftp\.ruby-lang\.org/pub/ruby/ruby\.taobao\.org/mirrors/ruby/g' ~/.rvm/config/db
```

## ruby 的安装与切换
- 列出已知的ruby版本
  ```
  rvm list known
  ```
- 安装一个 ruby 版本
  ```
  rvm list known
  ```
- 切换 ruby 版本
  ```
  rvm use 2.2.0
  ```
- 设置为默认版本
  ```
  rvm use 2.2.0 --default
  ```
- 卸载
  ```
  rvm remove 2.2.0
  ```