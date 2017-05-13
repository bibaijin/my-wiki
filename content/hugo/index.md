---
date: 2017-05-13T11:33:03+08:00
title: Hugo
---

一个静态网站生成器。

## 安装

```
go get -u -v github.com/kardianos/govendor
govendor get -v github.com/spf13/hugo
cd $GOPATH/src/github.com/spf13/hugo && go install
```

## 初始化工程

```
hugo new site ${project-name}
```

## 编辑

```
cd ${project-name}

# 添加主题
git clone https://github.com/digitalcraftsman/hugo-material-docs.git themes/hugo-material-docs

# 添加内容
hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>
```

## 测试

```
cd ${project-name}
hugo server
```
