---
title: win10 安装 mingw-w64
date: 2021-07-11 07:41:25
tags: 
    - C
---

Win10 搭建 C 开发环境

<!-- more -->

## mingw-w64

### 参考地址

官网 [http://mingw-w64.org/doku.php](http://mingw-w64.org/doku.php)

下载页面 [http://mingw-w64.org/doku.php/download](http://mingw-w64.org/doku.php/download)

软件包被托管在 SourceForge [https://sourceforge.net/projects/mingw-w64/files/mingw-w64/mingw-w64-release/](https://sourceforge.net/projects/mingw-w64/files/mingw-w64/mingw-w64-release/)


不要直接下载，滑动页面， 找到以下位置

![mingw.png](http://blog.image.codedemo.vip/mingw.png)


版本以及参数选择

版本及其他参数的含义参考文章 [MinGW-w64安装教程——著名C/C++编译器GCC的Windows版本](https://zhuanlan.zhihu.com/p/76613134)

本文以: `MinGW-W64 GCC-8.1.0 x86_64-win32-seh` 为例




## 安装配置

Step 1: 解压

Step 2: 复制 `mingw64` 到指定位置, 比如: `D:\Program Files`

Step 3: 添加环境变量, 如: `D:\Program Files\mingw64\bin`

Step 4: 使用命令 `gcc -v` 检查是否安装成功, 无报错信息即为安装成功

## Hello World

`hello_world.c`

```c
#include <stdio.h>

int main(int argc, char const *argv[])
{
    printf("%s\n", "Hello World");
    return 0;
}
```

编译

```bash
gcc hello_world.c -o hello_world.exe
```

运行

```bash
./hello_world.exe
```

