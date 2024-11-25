# cargo-generator使用教程

> 项目地址: https://github.com/cargo-generate/cargo-generate

## 项目介绍

cargo-generator是一个开发者工具, 通过利用预先存在的Git仓库作为模版, 帮助你快速启动一个新的Rust项目, 该项目使用Shopify的Liquid模版语言, Rhai用于钩子脚本, 正则表达式用于占位符

## 项目快速启动

### 安装

你可以通过以下命令安装cargo-generator

```bash
$ cargo install cargo-generator
或者
$ cargo binstall cargo-generator
```

### 使用

标准用法是传递一个`--git`标志给`cargo generator`, 或者简写为`cargo gen`, 这将提示你输入项目的名称:

```bash
$ cargo generate --git https://github.com/username-on-github/mytemplate.git
```

你也可以使用`--name`或`-n`标志直接传递项目名称:

```bash
$ cargo generate --git https://github.com/username-on-github/mytemplate.git --name myproject
```

你也可以不加`--git`参数, 直接传递给它一个本机的绝对路径的地址

