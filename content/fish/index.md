---
date: 2017-05-14T01:15:04+08:00
title: fish
---

一个用户友好的 Shell。

## 配置文件

- `~/.config/fish/config.fish` 与 `~/.config/fish/functions/*.fish` 自动加载。
- `~/.config/fish/functions/` 里的文件必须只包含一个函数。

## 语法

### 设置环境变量

```
set -x PATH $GOPATH/bin ~/.local/bin $PATH
```

### 设置别名

```
alias rmi="rm -i"
```

### 定义函数

```
function ll
    ls -l $argv
end
```
