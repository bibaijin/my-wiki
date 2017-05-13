---
date: 2017-05-13T11:33:03+08:00
title: Bootstrap
---

设置开发环境。

## 准备工作

- 安装 Virtual Box
- 安装 Vagrant

## 设置

```
git clone git@github.com:bibaijin/archlinux.git
cd archlinux/
vagrant up

# 进入虚拟机
vagrant ssh
sudo pacman -S go git
export GOPATH=~/Projects/go

mkdir -p ~/Projects/go/src/github.com/bibaijin
cd ~/Projects/go/src/github.com/bibaijin
git clone https://github.com/bibaijin/my-bootstrap.git
cd my-bootstrap/
go build
./my-bootstrap

# 重新登录
exit
vagrant ssh
```
