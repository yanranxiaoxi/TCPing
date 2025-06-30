[English](./README.md) | [简体中文](#)

# TCPing

⭐ 测试端口 TCP/HTTP 协议连通性命令行工具 ⭐

[![pipeline status](https://gitlab.soraharu.com/XiaoXi/TCPing/badges/master/pipeline.svg)](https://gitlab.soraharu.com/XiaoXi/TCPing/-/commits/master) [![Latest Release](https://gitlab.soraharu.com/XiaoXi/TCPing/-/badges/release.svg)](https://gitlab.soraharu.com/XiaoXi/TCPing/-/releases)

> 本工具源代码基于 [Cloverstd](https://github.com/cloverstd)/[tcping](https://github.com/cloverstd/tcping)，由 [@XiaoXi](https://soraharu.com/) 于 2021 年分叉并继续维护，中途合并部分原项目代码。

> 对于 IPv6 的支持来自于 [yuqaf1989](https://github.com/yuqaf1989) 在原项目提交的 [合并请求](https://github.com/cloverstd/tcping/pull/38)。

## 🤔 这是什么

一款能够便捷测试端口 TCP/HTTP 协议连通性的命令行工具，使用 Golang 编写，适配 Windows、MacOS、Linux、FreeBSD、DragonFly、AIX、illumos、Solaris 操作系统以及 x86、amd64、armv5、armv6、armv7、arm64、mips、mipsle、mips64、mips64le、riscv64、ppc64、ppc64le、loong64 处理器架构。

你可以在本项目的 [软件包库](https://gitlab.soraharu.com/XiaoXi/TCPing/-/packages/2) 找到适用的系统和架构的预编译二进制可执行文件。

## 🍭 使用说明

请 **自行编译** 或在本项目的 [软件包库](https://gitlab.soraharu.com/XiaoXi/TCPing/-/packages/2) 获取可执行文件。

**你可以使用该命令测试 TCP 端口：**

```shell
tcping soraharu.com 443
```

> 该命令将会测试 `soraharu.com` 服务器的 `443` 端口是否开放，如果指令结尾不指定端口号，则默认值 `80` 将会被使用

**你还可以使用以下命令测试 HTTP 服务：**

```shell
tcping -H soraharu.com
```

或者

```shell
tcping http://soraharu.com
```

> 以上命令将会测试 `http://soraharu.com:80` 是否允许连接

**其他帮助：**

你可以在 `tcping` 后添加参数 `-h` 或 `--help` 查看更多使用方法

```shell
tcping -h
```

## 🏃 默认参数

- `ping` 的默认次数为 `4`
- 如果不指定端口，则默认为 `80`
- `ping` 的默认时间间隔为 `1s`
- `ping` 的默认超时时间为 `1s`

## 📜 开源许可

基于 [MIT License](https://choosealicense.com/licenses/mit/) 许可进行开源。
