# 智能网页采集器（smart-crawler）

用一句自然语言描述需求，AI 自动爬取网页并输出结构化数据。基于 ScrapeGraphAI，支持本地模型运行，无 API 费用。

## 功能特点

- 自然语言描述即可采集，无需写爬虫规则
- 输出结构化数据（列表 / 表格 / JSON）
- 本地版可用 Ollama 模型，全程数据不出本机
- 适合电商信息、内容聚合、线索收集等场景

## 运行方式

```bash
pip install -r requirements.txt
streamlit run smart_crawler.py          # 云端版（OpenAI）
streamlit run local_crawler.py          # 本地版（Ollama，免 API）
```

云端版需配置 `OPENAI_API_KEY`；本地版需安装并运行 Ollama。

> 本项目仅供个人学习与技术交流使用（开源）。代码基于开源项目二次开发，遵循原项目对应的开源协议（Apache-2.0 / MIT），原始项目署名予以保留。
