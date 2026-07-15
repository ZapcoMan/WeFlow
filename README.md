<h1 align="center">WeFlow</h1>

<div align="center">
  <small>Forked from <a href="https://github.com/lurve1314/WeFlow" target="_blank">lurve1314/WeFlow</a></small>
</div>

<p align="center">
  <strong>完全本地、实时微信聊天记录查看、分析与导出工具</strong>
  <br>
  <img src="./app.jpg" alt="WeFlow应用截图" style="max-width: 80%; margin: 20px 0; border-radius: 8px;">
</p>

<p align="center">
  <a href="https://github.com/hicccc77/WeFlow/stargazers"><img src="https://img.shields.io/github/stars/hicccc77/WeFlow?style=flat&label=Stars&labelColor=2A3B4C&color=60A5FA" alt="Stargazers"></a>
  <a href="https://github.com/hicccc77/WeFlow/network/members"><img src="https://img.shields.io/github/forks/hicccc77/WeFlow?style=flat&label=Forks&labelColor=2A3B4C&color=60A5FA" alt="Forks"></a>
  <a href="https://github.com/hicccc77/WeFlow/releases"><img src="https://img.shields.io/github/downloads/hicccc77/WeFlow/total?style=flat&label=Downloads&labelColor=2A3B4C&color=60A5FA" alt="Downloads"></a>
  <a href="https://github.com/hicccc77/WeFlow/blob/main/LICENSE"><img src="https://img.shields.io/github/license/hicccc77/WeFlow?style=flat&label=License&labelColor=2A3B4C&color=60A5FA" alt="License"></a>
  <br>
  <a href="https://t.me/weflow_cc"><img src="https://img.shields.io/badge/Telegram-频道-60A5FA?style=flat&logo=telegram&logoColor=white&labelColor=2A3B4C" alt="Telegram Channel" style="height: 24px; vertical-align: middle;"></a>
  <a href="https://weflow.top"><img src="https://img.shields.io/badge/Website-官方网站-60A5FA?style=flat&logo=github&logoColor=white&labelColor=2A3B4C" alt="Website" style="height: 24px; vertical-align: middle;"></a>
</p>

<p align="center">
  <img src="https://api.star-history.com/badge?repo=hicccc77/WeFlow&theme=dark" alt="Star History Rank" style="height: 30px;">
</p>

<div align="center">
  
> [!IMPORTANT]
> **WeFlow 是完全本地的工具** - 所有数据处理都在用户本地完成，不会上传任何数据到服务器
> 
> **仅支持微信 4.0 及以上版本**

</div>

## 🚀 快速开始

### 普通用户
- **Windows**: 从 [Releases](https://github.com/hicccc77/WeFlow/releases) 下载 `.exe` 安装包
- **macOS**: 从 [Releases](https://github.com/hicccc77/WeFlow/releases) 下载 `.dmg` 文件
- **Linux**: 下载 `.AppImage` 或 `.tar.gz` 包
- **ArchLinux**: `yay -S weflow`

### 开发者
```bash
# 克隆项目
git clone https://github.com/lurve1314/WeFlow.git
cd WeFlow

# 安装依赖
npm install

# 启动开发环境
npm run dev

# 构建应用
npm run build
```

## ✨ 核心功能概览

| 类别 | 功能亮点 |
|------|----------|
| **📱 聊天查看** | 本地实时查看聊天记录，图片/视频/实况解密，消息防撤回 |
| **📊 数据分析** | 私聊分析、群聊画像、年度报告、双人报告、消息统计 |
| **📁 数据导出** | 支持 JSON、HTML、Markdown、Excel、CSV、ChatLab 等 10+ 格式 |
| **🌐 朋友圈** | 朋友圈内容预览/解密，图片/视频/实况查看，拦截删除操作 |
| **🔧 API 服务** | 本地 HTTP API (端口 5031)，提供 RESTful 接口供外部集成 |
| **🎙️ 智能功能** | 语音消息转文字 (sherpa-onnx)，AI 聊天洞察，群聊自动摘要 |

## 📋 详细功能清单

<details>
<summary><strong>点击查看完整功能列表</strong></summary>

### 🗨️ 聊天相关
- **本地实时聊天查看** - 无需网络，隐私安全
- **图片/视频/实况解密** - 支持微信原生加密格式
- **消息防撤回** - 防止他人消息被撤回
- **实时弹窗通知** - 新消息桌面提醒，支持黑白名单过滤
- **聊天记录修改** - 支持修改本地消息内容

### 📊 统计分析
- **私聊分析** - 消息数量统计、类型分析、发送比例、时段分布
- **群聊画像** - 群成员详情、发言排行、活跃时段、媒体内容统计
- **年度报告** - 按年生成统计报告，支持跨年度历史分析
- **双人报告** - 基于双方聊天记录生成专属分析报告
- **个人足迹** - 查看个人消息发送统计

### 📁 数据导出
- **多格式导出** - JSON、HTML、Markdown、TXT、Excel、CSV、PGSQL、ChatLab格式
- **批量导出** - 支持多个会话批量导出
- **增量导出** - 只导出新增内容
- **媒体文件导出** - 包含图片、视频等附件

### 🌐 朋友圈功能
- **内容解密** - 解密朋友圈图片、视频、实况
- **完整浏览** - 按时间线浏览所有朋友圈内容
- **导出功能** - 导出朋友圈文字和媒体内容
- **操作拦截** - 拦截朋友圈的删除与隐藏操作

### 🔧 开发与集成
- **HTTP API 服务** - 本地 RESTful API (端口 5031)
- **ChatLab 兼容** - 导出为 ChatLab 标准格式
- **实时推送** - Server-Sent Events (SSE) 实时消息推送
- **Webhook 支持** - 外部系统集成

### 🎙️ AI 智能功能
- **语音转文字** - 使用 sherpa-onnx 进行语音消息转录
- **AI 聊天洞察** - 自动生成聊天洞察和用户画像
- **群聊自动摘要** - 自动生成群聊内容摘要
- **智能搜索** - 基于内容的智能搜索

### 🔐 安全与隐私
- **完全本地** - 所有数据都在本地处理
- **密码锁屏** - 应用密码保护
- **Windows Hello** - 支持 Windows 生物识别解锁
- **隐私保护** - 无数据上传，尊重用户隐私

### 🛠️ 实用工具
- **联系人管理** - 导出好友、群聊、公众号信息
- **微信支付记录** - 查看微信支付历史
- **备份恢复** - 数据备份与恢复功能
- **多账号支持** - 支持多个微信账号管理

</details>

## 🖥️ 支持平台

| 平台 | 设备/架构 | 安装包格式 | 备注 |
|------|----------|-----------|------|
| **Windows** | Windows 10+，x64 | `.exe` (NSIS安装包) | 包含VC++运行时 |
| **macOS** | Apple Silicon (M系列，arm64) | `.dmg` | 支持M1/M2/M3芯片 |
| **Linux** | x64 (amd64) | `.AppImage`, `.tar.gz` | 主流发行版通用 |

## 🌐 HTTP API 服务

WeFlow 内置本地 HTTP API 服务，为开发者提供程序化访问接口：

```bash
# 默认启动地址
http://127.0.0.1:5031

# 示例：获取所有聊天会话
curl http://127.0.0.1:5031/api/sessions

# 示例：获取特定会话消息（支持SSE）
curl http://127.0.0.1:5031/api/sessions/123/messages?format=chatlab
```

**主要特性：**
- **RESTful 接口** - 标准的 REST API 设计
- **双格式支持** - 原始 JSON 或 ChatLab 标准格式
- **实时推送** - 基于 SSE 的实时消息推送
- **认证支持** - API 密钥认证（可选）
- **跨域支持** - 便于网页前端调用

📚 [查看完整 API 文档](docs/HTTP-API.md)

## 🏗️ 技术架构

WeFlow 基于现代技术栈构建，性能优异且功能丰富：

### 前端 (Renderer)
- **React 19** + **TypeScript** - 现代化的前端框架
- **Vite 8** - 极速构建工具
- **Zustand 5** - 轻量状态管理
- **ECharts 6** - 数据可视化图表
- **React Virtuoso** - 高性能虚拟列表

### 后端 (Main Process)
- **Electron 43** - 跨平台桌面框架
- **Koffi (FFI)** - 原生库调用 (WCDB, WeDecrypt, WeLive)
- **SQLite/WCDB** - 微信数据库引擎
- **Sherpa-onnx** - 本地语音识别
- **FFmpeg** - 视频处理

### 架构特点
- **多进程架构** - 主进程 + 渲染进程 + 8个Worker线程
- **原生集成** - 通过FFI直接调用微信原生库
- **完全离线** - 所有AI模型和依赖均在本地
- **模块化设计** - 45+ 服务模块，功能解耦清晰

## 📁 项目结构

```
WeFlow/
├── src/                    # 前端代码 (React + TypeScript)
│   ├── pages/             # 页面组件 (20+页面)
│   ├── components/        # 通用组件
│   ├── stores/           # Zustand状态管理
│   └── assets/           # 静态资源
├── electron/              # 后端代码 (Electron)
│   ├── main.ts           # 主进程入口 (171KB)
│   ├── services/         # 服务层 (45+模块)
│   ├── workers/          # Worker线程 (8个)
│   └── resources/        # 原生资源库
├── docs/                  # 文档
│   ├── HTTP-API.md       # API文档
│   ├── MAC-KEY-FAQ.md    # macOS密钥提取指南
│   └── CONTRIBUTING.md   # 贡献指南
└── resources/            # 平台特定资源
    ├── wcdb/            # WCDB原生库
    ├── wedecrypt/       # 解密库
    ├── welive/          # 实时监控库
    └── key/             # 密钥提取工具
```

## 🤝 贡献指南

欢迎贡献代码、报告问题或提出新功能建议！

### 开发流程
1. **Fork 项目**并创建特性分支
2. **编写代码**并确保测试通过
3. **提交代码**并创建 Pull Request
4. **代码审查**后合并

### 开发环境
```bash
# 安装依赖
npm install

# 开发模式运行
npm run dev

# 类型检查
npm run typecheck

# 构建应用
npm run build
```

### 代码规范
- 使用 TypeScript，严格类型检查
- 遵循项目现有的代码风格
- 添加必要的注释和文档
- 确保向后兼容性

## 📚 相关文档

- [📖 HTTP API 完整文档](docs/HTTP-API.md) - API 接口详细说明
- [🍎 macOS 密钥提取指南](docs/MAC-KEY-FAQ.md) - macOS 环境配置说明
- [🔧 开发者指南](docs/CONTRIBUTING.md) - 贡献代码指南
- [🌐 官方网站](https://weflow.top) - 项目官方网站

## 🙏 致谢

感谢以下项目为本项目提供技术支持：

- [密语 CipherTalk](https://github.com/ILoveBingLu/miyu) - 项目基础框架
- [WeChat-Channels-Video-File-Decryption](https://github.com/Evil0ctal/WeChat-Channels-Video-File-Decryption) - 视频解密技术参考
- [ChatLab](https://chatlab.fun/) - 聊天分析平台兼容格式

## 💌 联系与合作

如果您对 WeFlow 项目感兴趣，希望合作或咨询相关问题，欢迎联系我们：

<a href="mailto:yccccccy@proton.me"><img src="https://img.shields.io/badge/Email-yccccccy%40proton.me-60A5FA?style=flat-square&logo=proton&logoColor=white&labelColor=2A3B4C" alt="Protonmail" height="24px"></a>
<a href="https://t.me/weflow_cc"><img src="https://img.shields.io/badge/Telegram-频道-60A5FA?style=flat-square&logo=telegram&logoColor=white&labelColor=2A3B4C" alt="Telegram" height="24px"></a>

我们欢迎开源社区项目团队、开发者及其他合作伙伴与我们建立长期合作关系。

## 👥 贡献者

感谢所有为项目做出贡献的开发者！

<p align="center">
  <a href="https://github.com/hicccc77/WeFlow/graphs/contributors">
    <img src="https://contrib.rocks/image?repo=hicccc77/WeFlow" alt="Contributors" />
  </a>
</p>

---

<div align="center">
  
### ⚠️ 免责声明

**请负责任地使用本工具，遵守相关法律法规**  
WeFlow 是完全本地工具，不会上传任何用户数据。用户需对自己的行为负责。

### 📄 许可证

本项目基于 [MIT License](LICENSE) 开源。

---

**WeFlow** - 重新发现你的聊天记录 📱✨

</div>


