---
title: Mac终端配置
date: 2025-06-12 9:00:00
tags:
  - macOS
  - terminal
  - zsh
  - iTerm2
categories:
  - 工具
---

# 如何配置MAC终端

本文记录如何配置 macOS 终端（使用 Oh-My-Zsh 和 Powerlevel10k）

---

## 安装 Homebrew

打开终端，运行以下命令安装 Homebrew：

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

安装完成后，添加 Homebrew 至环境变量：

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

---

## 安装 iTerm2

安装 iTerm2：

```bash
brew install --cask iterm2
```

后续操作建议在 iTerm2 中执行。

---

## 安装 Git

可通过安装Xcode Command Line Tools获取，

也可使用 Homebrew 安装：

```bash
brew install git
```

---

## 安装 Oh My Zsh

通过以下命令安装 Oh My Zsh：

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

---

## 安装 Powerlevel10K 主题

克隆主题到本地：

```bash
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

编辑 `~/.zshrc`，修改主题：

```zsh
ZSH_THEME="powerlevel10k/powerlevel10k"
```

使更改立即生效：

```bash
source ~/.zshrc
```

---

## 安装 Meslo Nerd Font

安装 Meslo Nerd 字体，并在 iTerm2 中选择，安装过程中可能会提示按 `y` 键确认。

---

## 更新 VSCode 终端字体

如果使用 VSCode 的终端，编辑用户 `settings.json`，添加：

```json
"terminal.integrated.fontFamily": "MesloLGS NF"
```

---

## 配置 PowerLevel10K

重启 iTerm2，你会看到 PowerLevel10K 的配置向导；如果没有出现，可手动运行：

```bash
p10k configure
```

并按提示完成配置，使终端外观最佳。

---

## 安装 ZSH 插件

### 安装 zsh-autosuggestions

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ~/.oh-my-zsh/plugins/zsh-autosuggestions
```

### 安装 zsh-syntax-highlighting

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ~/.oh-my-zsh/plugins/zsh-syntax-highlighting
```

编辑 `~/.zshrc`，修改插件列表：

```zsh
plugins=(git zsh-autosuggestions zsh-syntax-highlighting web-search)
```

最后运行：

```bash
source ~/.zshrc
```
