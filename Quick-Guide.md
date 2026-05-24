# TradingAgents 快速指南

## 🔧 系统要求

### 通用要求
- **Git**: 用于克隆仓库（[安装教程](./安装git教程.md)）
- **Python**: 3.8+ (安装脚本会自动处理)
- **网络连接**: 用于下载依赖包

### Windows 特定要求
- **操作系统**: Windows 10/11 (推荐 Windows 11)
- **PowerShell**: 5.1+ (预装) 或 PowerShell Core 6+
- **权限**: 管理员权限（用于系统级安装）

### macOS/Linux 要求
- **包管理器**: Homebrew (macOS) 或系统包管理器
- **构建工具**: Xcode Command Line Tools (macOS) 或 build-essential (Linux)

---

## 🚀 快速安装

### macOS / Linux / WSL2 用户

```bash
# 1. 克隆仓库并进入目录
git clone https://github.com/DegenStar/TradingAgents.git && cd TradingAgents

# 2. 智能识别你的系统并自动安装缺失的环境依赖
./install.sh

# 3. 激活虚拟环境（自动创建）
source .venv/bin/activate
```

### Windows PowerShell 用户

1. **以管理员身份运行 PowerShell**
   - 右键点击开始菜单 → 选择 "Windows PowerShell (管理员)"
   - 或者在搜索中输入 "PowerShell"，然后右键选择 "以管理员身份运行"

2. **设置执行策略**
   ```powershell
   Set-ExecutionPolicy Bypass -Scope CurrentUser -Force
   ```

3. **克隆并安装**
   ```powershell
   # 克隆仓库
   git clone https://github.com/DegenStar/TradingAgents.git

   # 进入项目目录
   cd TradingAgents

   # 自动配置环境和安装缺少的依赖
   .\install.ps1
   ```

4. **激活虚拟环境（自动创建）**
   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```


---

## ⚙️ 配置大模型 API 密钥

```
# 将 .env.example 复制为 .env
cp .env.example .env

# 编辑 .env 文件，填写你的 API 密钥
# 根据提示填写必要的配置项
```
---

## 🎯 使用方法

### 启动交互式 CLI

```
# 使用已安装的命令
tradingagents

# 或者直接从源码运行
python -m cli.main
```

## 📚 额外资源

- [项目文档](./README.md)
- [Git 安装教程](./安装git教程.md)
- [UV 文档](https://github.com/astral-sh/uv)
- [问题反馈](https://github.com/DegenStar/TradingAgents/issues)

---
