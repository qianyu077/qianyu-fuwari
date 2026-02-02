---
title: xray-xhttp
published: 2026-02-02
description: xhttp脚本的部署教程
image: ''
tags: [xray, xhttp, 部署, vps, lxc]
category: 技术教程
draft: false 
lang: zh-CN
---

# xhttp脚本部署教程

## 准备工作

首先，你需要准备一台服务器，可以是VPS或者LXC小鸡，具体选择取决于你的个人需求。本教程将使用拼好鸡家的美国LXC小鸡进行演示，该小鸡提供三网骨干直连，网络质量优秀。

## 部署步骤

### 1. SSH登录服务器

使用SSH工具登录到你的服务器，例如使用终端命令：

```bash
ssh root@your-server-ip
```

### 2. 下载并运行一键部署脚本

复制并执行以下命令，下载并运行GitHub中Xray-script项目的一键部署脚本：

```bash
wget --no-check-certificate -O ${HOME}/xray-script.sh https://raw.githubusercontent.com/zxcvos/Xray-script/main/install.sh && bash xray-script.sh
```

执行命令后，脚本会自动下载并开始运行，如图所示：

![下载脚本](/xray-xhttp_1.png)

### 3. 按照提示完成部署

脚本运行后，会显示安装过程和相关依赖的配置，如图所示：

![安装依赖](/xray-xhttp_2.png)

安装完成后，脚本会显示主菜单界面，如图所示：

![脚本主菜单](/xray-xhttp_3.png)

### 4. 配置选项

在部署过程中，脚本会提示你进行一些配置选择：

- **协议选择**：推荐使用默认协议
- **端口设置**：默认端口为443
- **其他选项**：根据个人需求进行调整

### 5. LXC小鸡特殊设置

如果你使用的是LXC小鸡，需要注意将443端口映射出去，以确保服务能够正常访问。

## 部署完成

按照脚本提示完成所有配置后，xhttp服务会自动启动并运行在你指定的端口上。你可以使用脚本主菜单中的相关选项来管理和查看服务状态。

## 总结

通过本教程的步骤，你可以轻松在VPS或LXC小鸡上部署xhttp脚本，享受稳定的网络服务。如果在部署过程中遇到问题，可以参考GitHub项目页面的相关文档或提交Issue寻求帮助。

---

**项目地址**：[https://github.com/qianyu077/Xray-script](https://github.com/qianyu077/Xray-script)