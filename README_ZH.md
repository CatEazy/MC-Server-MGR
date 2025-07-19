[English](README.md) | 简体中文

# MC服务器管理器

现在由Python驱动！（原批处理版本已移至 `old/` 文件夹）

# ✨ 特点

- 小巧轻快
- 跨平台支持（Windows、Linux、macOS）
- 常用配置更改方便
- 用户友好的配置界面
- 自动处理EULA协议
- 还有其他...

# 📦 快速开始

**系统要求：**
- Python 3.6 或更高版本
- Java（用于运行Minecraft服务器）

**安装步骤：**
1. 下载或克隆此仓库
2. 确保在同一目录下有Minecraft服务器jar文件（例如 `server.jar`）
3. 运行程序：
   - **Windows**: 双击 `start.bat` 或运行 `python start.py`
   - **Linux/macOS**: 运行 `./start.sh` 或 `python3 start.py`

程序会自动创建配置文件并处理EULA协议。你只需要有一个服务器核心文件就可以开始使用了。

# 🔧 从源码构建

如果您想自己构建可执行文件：

**前置要求：**
- Python 3.6 或更高版本
- Nuitka（会自动安装）

**构建说明：**

1. **自动构建（推荐）：**
   - **Windows**: 运行 `build.bat`
   - **Linux/macOS**: 运行 `./build.sh`

2. **手动构建：**
   ```bash
   # 安装Nuitka
   pip install nuitka ordered-set
   
   # 构建（单文件）
   python -m nuitka --standalone --onefile --output-filename=mc-server-manager --enable-plugin=no-qt --assume-yes-for-downloads --output-dir=dist start.py
   ```

3. **使用构建脚本：**
   ```bash
   python build.py
   ```

**GitHub Actions：**
本项目包含通过GitHub Actions的自动构建。每次发布时会自动为Windows、Linux和macOS构建可执行文件。

# 愿望单

- [ ] 多语言支持
- [x] 跨平台Python版本
- [ ] 图形用户界面
- [ ] 插件管理
- [ ] 备份功能
- [ ] 更多...

# 作者B站

[点我！](https://space.bilibili.com/3546703915387263)
