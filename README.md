# 听记 ListenRecord

<img src="assets/logo.png" width="88" height="88" alt="ListenRecord">

**录音、实时转写、AI 纪要，一个应用全搞定** · Tauri 2 · Vue 3 · Rust

[**中文**](README.md) | [English](README.en.md)

[![Latest Release](https://img.shields.io/github/v/release/Linlx0628/listenrecord-app?label=Latest%20Release)](https://github.com/Linlx0628/listenrecord-app/releases/latest)
[![Platforms](https://img.shields.io/badge/Platforms-macOS%20%7C%20Windows%20%7C%20Linux%20%7C%20Android-4c566a)](https://github.com/Linlx0628/listenrecord-app/releases/latest)
[![License](https://img.shields.io/badge/License-Proprietary-8b8b8b)](#反馈与许可)

![听记 ListenRecord](assets/banner.webp)

> 会议、访谈、课程，录完就有文字、有摘要、有待办。**语音识别在本机运行，原始音频不需要上传。**

[**⬇︎ 下载最新版本**](https://github.com/Linlx0628/listenrecord-app/releases/latest) · [官网](https://www.lingerx.cn) · [更新日志](CHANGELOG.md) · [反馈问题](https://github.com/Linlx0628/listenrecord-app/issues)

## 亮点

- **本地语音识别** —— 模型下载后识别在本机进行，录音不上传也能出文字
- **会议双流** —— 麦克风和电脑声音分开识别，我方发言与对方声音分得清
- **AI 纪要** —— 内置 10 类摘要模板，输出议题、决策、风险与行动项
- **AI 思维导图 · 段落总结 · 翻译**
- **说话人识别** —— 自动区分发言人，转写带时间戳，可回放定位
- **Agent 接入** —— 摘要与任务可以只读方式提供给 Codex、Claude Code 等终端 Agent
- **加密同步** —— 会议与任务跨设备同步，端到端加密，改密码无需重加密历史记录
- **全平台** —— macOS Apple Silicon / Windows x64 / Linux x86_64 / Android arm64
- **飞书文档与任务同步 · 多格式导出**

## 界面预览

|  |  |
|:--:|:--:|
| ![首页](assets/screenshots/01-home.webp) | ![录音入口](assets/screenshots/02-recording-actions.webp) |
| **首页** —— 录音、任务与日程的统一入口 | **录音入口** —— 速记、翻译、文件转写与录音记录 |
| ![实时转写](assets/screenshots/03-live-transcription.webp) | ![转写内容](assets/screenshots/04-transcript.webp) |
| **实时转写** —— 边录边转，波形与流式识别状态实时可见 | **转写内容** —— 时间戳与说话人分离，可回放定位 |
| ![摘要模板](assets/screenshots/05-summary-templates.webp) | ![AI 摘要](assets/screenshots/06-summary.webp) |
| **摘要模板** —— 内置 10 类模板，按会议类型选择 | **AI 摘要** —— 输出议题、决策、风险与行动项 |
| ![AI 思维导图](assets/screenshots/07-mindmap.webp) | ![任务列表](assets/screenshots/08-tasks.webp) |
| **AI 思维导图** —— 把会议结构展开成可导出的导图 | **任务列表** —— 从会议中提取的待办，带优先级与截止时间 |
| ![日程](assets/screenshots/09-calendar.webp) | 更多界面与交互演示见官网<br>[https://www.lingerx.cn](https://www.lingerx.cn) |
| **日程** —— 月视图汇总录音、任务与 AI 总结 | |

## 下载

请始终从 [Latest Release](https://github.com/Linlx0628/listenrecord-app/releases/latest) 获取当前公开版本，不要根据历史命名规则猜测附件地址。

| 平台与架构 | 安装包 | 应用内更新 | 安装提示 |
|------------|--------|------------|----------|
| macOS Apple Silicon（aarch64） | [DMG](https://github.com/Linlx0628/listenrecord-app/releases/latest) | 支持 | 系统音频需要屏幕录制权限；首次打开时也可能出现 macOS 安全提示，请核对下载来源后按系统指引处理。 |
| Windows x64 | [NSIS EXE](https://github.com/Linlx0628/listenrecord-app/releases/latest) | 支持 | 下载后运行安装程序；若系统显示安全提示，请先核对发布者与下载来源。 |
| Linux x86_64 / amd64 | [AppImage / DEB](https://github.com/Linlx0628/listenrecord-app/releases/latest) | 支持 | AppImage 可能需要添加执行权限；系统音频能力取决于本机 PulseAudio/PipeWire 环境。应用内更新使用的就是官网下载的同一个 AppImage 文件。 |
| Android（`arm64-v8a`） | [APK](https://github.com/Linlx0628/listenrecord-app/releases/latest) | 不使用桌面 updater | 侧载时需要允许“安装未知来源应用”，请仅对可信下载来源授权。 |

## 更多

- **工程笔记** —— 为什么选 Tauri 2、流式 ASR 如何工作、三套系统音频栈、加密同步的信封设计、Android 的 `DT_NEEDED` 坑、发布工程：[TECHNICAL.md](TECHNICAL.md)
- **版本变更**：[CHANGELOG.md](CHANGELOG.md)
- **安全漏洞报告**：[SECURITY.md](SECURITY.md)

## 边界说明

- 定位是**本地优先，不是完全离线**：首次下载模型、在线 AI、账号与权益、加密同步、飞书、邮件和更新检查按需联网
- 桌面端支持系统音频录制与会议双流；Android 与 iOS 不支持，移动端不是桌面能力的完整复刻
- 请只从本仓库 [Releases](https://github.com/Linlx0628/listenrecord-app/releases) 或官网 [www.lingerx.cn](https://www.lingerx.cn) 下载

## 反馈与许可

- 反馈与合作：[GitHub Issues](https://github.com/Linlx0628/listenrecord-app/issues) · [listennote@lingerx.cn](mailto:listennote@lingerx.cn)
- 本仓库是**二进制分发仓库**：不含应用源代码，也不等同于以任何开源许可证授权
- 具体权利与限制以正式软件许可和服务条款为准
