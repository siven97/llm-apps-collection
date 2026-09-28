# 语音客服助手（voice-desk）

基于自有知识库的语音客服：Firecrawl 爬取文档站点 → Qdrant 建向量知识库 → GPT-4o 生成回答 → OpenAI TTS 语音播报，支持文字与语音双通道。

## 功能特点

- 知识库构建：自动爬取文档站点并建索引（Firecrawl + Qdrant + FastEmbed）
- 智能问答：基于知识库生成清晰、准确的回答
- 语音播报：多音色 OpenAI TTS，语速语气自然
- 音频下载：回答可下载为音频文件
- Streamlit 界面，侧边栏配置 API

## 运行方式

```bash
pip install -r requirements.txt
streamlit run voice_desk_agent.py
```

需配置：`OPENAI_API_KEY`、Qdrant 地址与 API Key、Firecrawl API Key（页面或环境变量均可）。

> 本项目仅供个人学习与技术交流使用（开源）。代码基于开源项目二次开发，遵循原项目对应的开源协议（Apache-2.0 / MIT），原始项目署名予以保留。
