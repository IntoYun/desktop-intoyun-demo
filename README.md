# 基于`IntoYun第三方设备SDK`开发的桌面系统实例工程

通过该项目，我们将介绍如何使用`IntoYun第三方设备SDK`开发第三方设备。

该项目工程使用intoyuniot开发工具开发。


## 目录和文件组成

```
+-- lib                       : 库目录
+-- src                       : 源文件目录
    +-- components            : 插件文件夹
        +-- intoyun_iot       : 第三方设备SDK
    +-- user                  : 用户应用代码
+-- intoyuniot.ini            : intoyuniot配置文件
+-- README.md                 : 项目说明文件

```

## 下载工程

```
git clone --recursive https://github.com/IntoYun/desktop-intoyun-demo.git
```

## 项目实例开发

- [Linux硬件平台](#1-linux硬件平台)
- [MacOS硬件平台](#2-macos硬件平台)
- [Windows硬件平台](#3-windows硬件平台)

### 1 Linux硬件平台

#### 1.1 程序编译

```
intoyuniot run -t clean              # 清除临时文件

intoyuniot run -e linux_x86_64       # 编译64位程序
或
intoyuniot run -e linux_i686         # 编译32位程序

```

#### 1.2 程序运行

```
./.intoiotenvs/linux_x86_64/program
或
./.intoiotenvs/linux_i686/program
```

### 2 MacOS硬件平台

#### 2.1 程序编译

```
intoyuniot run -t clean              # 清除临时文件
intoyuniot run -e native             # 编译程序
```

#### 2.2 程序运行

```
./.intoiotenvs/native/program
```

### 3 Windows硬件平台

#### 3.1 程序编译

```
intoyuniot run -t clean              # 清除临时文件
intoyuniot run -e windows_x86        # 编译程序
```

#### 3.2 程序运行

```
./.intoiotenvs/windows_x86/program
```

