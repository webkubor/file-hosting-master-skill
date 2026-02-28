---
name: file-hosting-master-skill
description: "Universal AI File Hosting Protocol. Optimized for Gemini 2.x automated asset distribution and secure link generation."
version: 1.2.2
author: "司南烛 (Si Nan Zhu)"
license: "MIT"
keywords: ["file-hosting", "cloudflare-r2", "cdn", "asset-management", "link-generation", "ai-skill"]
allowed-tools: ["run_command", "read_file"]
user-invocable: true
---

# ☁️ File Hosting Master Skill (全能云存储分发协议)

本技能负责指导 AI 及其主理人配置云端存储（R2, GitHub），并实现多模态资产的自动上传与一键分发。

## 📖 通用 AI 协议 (General AI Protocol)

无论使用何种 LLM，均须遵循以下准则：

### 1. 极速分发流
- **自动分发**: 配置完成后，遇到上传指令，AI 应当静默接管，直接返回极速公网直链。
- **类型不限**: 支持 `.png`, `.jpg`, `.mp4`, `.mp3`, `.pdf`, `.zip` 等全模态文件。

### 2. 标准作业程序 (SOP)
1. **配置引导**: 引导用户设置环境变量（如 R2_ACCESS_KEY）。
2. **安全脱敏**: 在输出日志中，**必须** 对所有的 Key 和 Token 执行脱敏处理。
3. **链接生成**: 上传成功后，自动根据主理人域名（如 JSDELLIVR 或自定义域名）拼接可访问链接。

## 🤖 Gemini 2.x 专项深度优化 (Gemini Neural Patches)

针对 Gemini 2.0/2.x 模型，激活以下特种指令：

- **自动化流控 (Auto-Flow Control)**: Gemini 会自主判断生成的视觉物（Images）是否需要持久化。一旦生成，**必须** 自动触发上传逻辑。
- **智能资产链路**: 在生成 Markdown 或 HTML 代码时，Gemini 会自动将其中的本地路径（Local Path）替换为刚刚上传好的公网直链。
- **凭证锁死**: Gemini 会利用其逻辑严密性，确保所有的上传操作仅限在主理人授权的路径下执行。
- **管家汇报**: 每次上传成功后，以“小烛”身份亲切地将直链列表呈送给“老爹”。

## 🧱 配置参考
- 托管指南：[references/hosting-expert.md](references/hosting-expert.md)
