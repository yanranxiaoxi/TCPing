[English](#) | [简体中文](./README.zh-Hans.md)

# TCPing

⭐ Command line tool to test port TCP/HTTP protocol connectivity ⭐

[![pipeline status](https://gitlab.soraharu.com/XiaoXi/TCPing/badges/master/pipeline.svg)](https://gitlab.soraharu.com/XiaoXi/TCPing/-/commits/master) [![Latest Release](https://gitlab.soraharu.com/XiaoXi/TCPing/-/badges/release.svg)](https://gitlab.soraharu.com/XiaoXi/TCPing/-/releases)

> The source code for this tool is based on [Cloverstd](https://github.com/cloverstd)/[tcping](https://github.com/cloverstd/tcping), which was created by [@XiaoXi](https://soraharu.com/) in Forked in 2021 and continues to be maintained, merging some of the original project code halfway through.

> Support for IPv6 comes from a [pull request](https://github.com/cloverstd/tcping/pull/38) submitted by [yuqaf1989](https://github.com/yuqaf1989) in the original project.

## 🤔 What is this

A command line tool to easily test port TCP/HTTP protocol connectivity, written in Golang for Windows, MacOS, Linux, FreeBSD, DragonFly, AIX, illumos, Solaris and x86, amd64, armv5, armv6, armv7, arm64, mips, mipsle, mips64, mips64le, riscv64, ppc64, ppc64le, loong64 processor architectures.

You can find pre-compiled binary executables for applicable systems and architectures in the [package repository](https://gitlab.soraharu.com/XiaoXi/TCPing/-/packages/2) for this project.

## 🍭 Instructions for Use

Please **compile it yourself** or get the executable from the [package repository](https://gitlab.soraharu.com/XiaoXi/TCPing/-/packages/2) of this project.

**You can use this command to test TCP ports:**

```shell
tcping soraharu.com 443
```

> This command will test if the `soraharu.com` server's `443` port is open or not, if the port number is not specified at the end of the command, the default value of `80` will be used

**You can also test the HTTP service using the following command:**

```shell
tcping -H soraharu.com
```

or

```shell
tcping http://soraharu.com
```

> The above command will test if `http://soraharu.com:80` is allowed to connect.

**Other help:**

You can add the parameter `-h` or `--help` after `tcping` to see how to use it.

```shell
tcping -h
```

## 🏃 Default Parameters

- The default number of `ping`s is `4`.
- If no port is specified, the default is `80`.
- The default time interval for `ping` is `1s`.
- The default timeout for `ping` is `1s`.

## 📜 Open Source License

Open source based on the [MIT License](https://choosealicense.com/licenses/mit/) license.
