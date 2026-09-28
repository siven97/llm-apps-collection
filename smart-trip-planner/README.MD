# 智能行程规划助手（smart-trip-planner）

输入目的地、天数、预算，AI 自动研究并生成个性化旅行行程，支持导出 `.ics` 日历文件，一键导入 Google / Apple / Outlook 日历。

## 功能特点

- 目的地调研：自动搜索景点、活动、住宿信息
- 个性化行程：按天数与偏好生成逐日安排
- 日历导出：生成 `.ics` 文件，含每日活动完整描述
- 双版本：云端 GPT-4o 版 / 本地 Ollama 版（免 API）

## 运行方式

```bash
pip install -r requirements.txt
streamlit run trip_planner.py          # 云端版（OpenAI + SerpAPI）
streamlit run local_trip_planner.py    # 本地版（Ollama，免 OpenAI）
```

需配置：`OPENAI_API_KEY`（云端版）、SerpAPI Key（联网搜索）；本地版需安装并运行 Ollama。

> 本项目仅供个人学习与技术交流使用（开源）。代码基于开源项目二次开发，遵循原项目对应的开源协议（Apache-2.0 / MIT），原始项目署名予以保留。
