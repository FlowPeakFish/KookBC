# KookBC (Kook Bot Client)

这是一个 [JKook API](https://github.com/SNWCreations/JKook) 的标准 Java 客户端实现。

## 用法

从右侧 Releases 下载最新版本。

* **如果可能，请始终使用最新版本！**

下载后，请将下载的 KookBC 程序，以及您将要使用的 基于 JKook API 的 Java Bot 程序 一同放在一个全新目录里。

然后用如下命令行启动 KookBC:

```text
java -jar kookbc-<version>.jar
```

其中，`<version>`是 KookBC 的版本。

之后，KookBC 会在当前目录下生成一个名为 kbc.yml 的 KookBC YAML 配置文件并退出。

更详细的命令行选项见 [KookBC 命令行](docs/KookBC_CommandLine.md) 。

配置内容详解请见 [KookBC YAML 配置详解](docs/KookBC_Config.md) 。请按照文档的解释，配置您的 KookBC 。

配置完成后，再次使用之前的命令行启动 KookBC ，当如下语句出现时，您的 Kook 机器人就已经准备就绪，可以使用。

```text
[XX:XX:XX] [Main thread/INFO] Done! (XXs) Type "help" for help.
```

其中，`X` 为任意可能的值，您可以忽视。

更多 KookBC 的命令行选项可以通过以下命令获得:

```text
java -jar kookbc-<version>.jar --help
```

其中，`<version>`是 KookBC 的版本。

## 贡献

很感谢您愿意帮助我们改进 KookBC ！

您有两种贡献方法:
* 提出 Issue
* 提出 Pull Request

您可以在 Issues 提出您使用 KookBC (不包括其搭载的 Bot 程序) 的过程中遇到的问题，包括但不限于 KookBC 的程序错误，漏洞，或文档错误等。

如果您会 Java 编程 ，并且希望帮助我们改进 KookBC 的程序，请按照以下过程进行您的 Pull Request 过程:
* 创建一份此仓库的 Fork
* 从 dev 分支签出您的 Fork 分支，以 `fork-<您的 Github 用户名>` 命名
* 在其中做好您的修改
* 提交，并 Push 到您的 Fork
* 根据 Pull Request Template ，向我们发出 Pull Request
* 等待我们审核
* 若不同意，根据我们的修改意见做出改进，并请求继续
* 或通过，并被并入 dev 分支，若到这里，您的 Pull Request 过程就宣告结束

上述过程对文档的修改也适用，~~但请从 doc 分支签出~~。**我们不再使用 doc 分支，其已经于 2022/8/18 删除。**

但是，Pull Request 的提出遵循一个原则: **一个 Pull Request 只解决一个问题。**
如一个 Fork 同时解决了文档错误和程序错误，则应该分别提出 Pull Request。

## 技术信息

网络通信库: OkHttp 3

JSON 处理库: Google GSON

控制台功能库: JLine 3, TerminalConsoleAppender

日志库: Apache Log4j2

## 版权

此程序使用 AGPLv3 作为许可证。
