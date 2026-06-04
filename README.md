# AI 对话阅读器

一个轻量的单文件 HTML 工具，用于离线阅读和浏览 AI 对话记录。

## 支持的格式

| 来源 | 文件格式 | 说明 |
|------|----------|------|
| ChatGPT | `.json` | 从 ChatGPT 导出的对话文件 |
| Claude Code | `.jsonl` | Claude Code CLI 的会话日志 |
| Codex | `rollout*.jsonl` | OpenAI Codex 的 rollout 日志 |

## 使用方式

1. 直接在浏览器中打开 `viewer.html`
2. 将文件拖拽到页面上，或点击「选择文件」按钮
3. 浏览对话内容

## 功能特性

- 气泡式对话界面，用户/助手消息左右分列
- 内置 Markdown 渲染（标题、列表、表格、代码块等）
- 折叠面板展示工具调用详情和返回结果
- 显示思考过程（thinking）和推理摘要
- 展示 token 用量统计
- 大文件分批渲染，避免页面卡顿
- 纯前端，无需服务器，无外部依赖

## 项目结构

```
.
├── viewer.html          # 主程序（单文件，包含 HTML/CSS/JS）
├── sessions/            # 示例会话文件（已 gitignore）
└── README.md
```
