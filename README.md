# TCPing

⭐ 测试端口 TCP/HTTP 协议连通性命令行工具 ⭐

## 🤔 这是什么

一款能够便捷测试端口 TCP/HTTP 协议连通性的命令行工具，使用 Golang 编写，适配 Windows、Linux、FreeBSD 操作系统以及 x86、amd64、arm、arm64、mips、mipsle 处理器架构。

你可以在本项目的 [发布页面](https://gitlab.soraharu.com/XiaoXi/TCPing/-/releases) 找到适用的系统和架构版本。

## 🍭 使用说明

**你可以使用该指令测试 TCP 端口：**

```shell
tcping soraharu.com 443
```

*该指令将会测试 `soraharu.com` 服务器的 `443` 端口是否开放，如果指令结尾不指定端口号，则默认值 `80` 将会被使用

**你还可以使用以下指令测试 HTTP 服务：**

```shell
tcping -H soraharu.com
```

或者

```shell
tcping http://soraharu.com
```

*以上指令将会测试 `http://soraharu.com:80` 是否允许连接

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
