# QwenPaw Portable Build

自动从 [agentscope-ai/QwenPaw](https://github.com/agentscope-ai/QwenPaw) 上游 release 构建便携版安装包。

## 工作原理

1. **每 2 小时**自动检查上游 release
2. 发现新版本后自动构建 Windows / Linux 便携版
3. 构建产物自动发布到 [Releases](https://github.com/hllshiro/qwenpaw-portable/releases)
4. 也支持手动触发，指定任意上游 tag

## 下载

前往 [Releases](https://github.com/hllshiro/qwenpaw-portable/releases) 页面下载最新版本。

---

## 使用说明

### Windows

1. 下载 `qwenpaw-portable-win-x64-v*.zip`
2. 解压到任意目录
3. 打开命令提示符，进入解压目录

```cmd
# 启动服务
qwenpaw.bat app
```

### Linux

1. 下载 `qwenpaw-portable-linux-x64-v*.tar.gz`
2. 解压并进入目录

```bash
tar -xzf qwenpaw-portable-linux-x64-v*.tar.gz
cd qwenpaw-portable-linux

# 启动服务
./qwenpaw.sh app
```

### 更多用法

请参考 QwenPaw 官方文档：https://docs.qwenpaw.ai

---

## 便携版特点

- 无需安装 Python / Node.js
- 内含 Python 运行时 + 预编译依赖
- 解压即用

## 致谢

本项目不修改 QwenPaw 源码，仅提供构建打包服务。QwenPaw 由 [agentscope-ai/QwenPaw](https://github.com/agentscope-ai/QwenPaw) 团队开发。
