---
title: Mac前端开发环境配置
date: 2025-06-14 12:00:00
tags:
  - macOS
categories:
  - 工具
---

# 如何配置MAC前端开发环境

本文记录如何配置 macOS 前端开发环境

---

## 安装 Nvm

1.通过brew安装 Nvm：

```bash
brew install nvm
```

2.创建 Nvm 工作目录：
```bash
mkdir ~/.nvm
```

3.配置 .zshrc：
```bash
# nvm config
export NVM_DIR="$HOME/.nvm"
# This loads nvm
[ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"
# This loads nvm bash_completion
[ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"
```

## 安装 bun

1.通过curl安装 bun：
```bash
curl -fsSL https://bun.sh/install | bash
```

2.配置 .zshrc：
```bash
# bun config
export BUN_INSTALL="$HOME/.bun"
export PATH="$BUN_INSTALL/bin:$PATH"
```

3.卸载 bun：
```bash
rm -rf ~/.bun
```

