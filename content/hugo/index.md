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

cd ${project-name}
# 在 config.toml 中添加 publishDir = "docs"
```

## 编辑

```
cd ${project-name}

# 添加主题
git submodule add https://github.com/digitalcraftsman/hugo-material-docs.git themes/hugo-material-docs

# 添加内容
hugo new <SECTIONNAME>/<FILENAME>.<FORMAT>
```

## 测试

```
cd ${project-name}
hugo server
```

## 发布

```
cd ${project-name}
hugo  # 更新 docs/ 文件夹
git push origin master  # 发布
```
