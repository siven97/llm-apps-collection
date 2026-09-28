# 对话式图表工作台（chart-chat-studio）

聊天即可生成实时图表、指标与数据面板的 Next.js 仪表盘（生成式 UI）。Agent 把图表作为画布上的"可寻址产物"持续创建与更新，而不只是输出文字。

## 功能特点

- 聊天生成实时图表 / KPI / 指标面板
- 画布持久化：Agent 可跨轮次更新、重排图表
- 基于 CopilotKit + AG-UI + ADK 的 Agent 架构
- 简洁聊天侧栏 + 主画布布局

## 运行方式

```bash
pnpm install
cp .env.example .env    # 填入你的 GOOGLE_API_KEY
pnpm dev
```

环境要求：Node.js 18+、Python 3.8+（ADK Agent）、Google AI Studio 的 API Key。

> 本项目仅供个人学习与技术交流使用（开源）。代码基于开源项目二次开发，遵循原项目对应的开源协议（Apache-2.0 / MIT），原始项目署名予以保留。
