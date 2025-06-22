---
title: Mac 常用应用安装指南
date: 2025-06-22 21:00:00
tags:
  - macOS
  - 应用安装
  - 开发工具
categories:
  - 工具
---

# Mac 常用应用安装指南

本文记录在 macOS 系统上安装常用应用程序的详细步骤，包括开发工具、办公软件和实用工具。

---

## 🛠️ 开发工具

### 1. Homebrew - 包管理器

Homebrew 是 macOS 上最流行的包管理器，建议首先安装：

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

安装完成后配置环境变量：

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

## 📄 办公软件

### 1. Microsoft Office 批量许可版本

> ⚠️ **注意**：此方法仅供学习和测试使用，商业用途请购买正版授权。

> 具体参考：https://github.com/alsyundawy/Microsoft-Office-For-MacOS

1. **下载 Office 安装包**
   - 访问：https://go.microsoft.com/fwlink/?linkid=525133
   - 下载 Microsoft Office LTSC 2024 for Mac

2. **安装 Office 应用**
   ```bash
   # 下载完成后双击安装包进行安装
   ```

3. **激活工具**
   - 下载地址：https://github.com/alsyundawy/Microsoft-Office-For-MacOS/blob/master/DATA/Microsoft_Office_LTSC_2024_VL_Serializer.pkg
   - 运行激活工具完成激活

4. **许可证管理**
   - 如需删除许可证：https://go.microsoft.com/fwlink/?linkid=849815

---

## 🛠️ 实用工具

### 1. 系统增强工具

#### AppCleaner - 应用清理
```bash
brew install --cask appcleaner
```

---

## 📚 相关资源

- [Homebrew 官方文档](https://brew.sh/)
- [Microsoft Office for Mac 官方支持]()

---
