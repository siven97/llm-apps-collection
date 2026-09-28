# 自校验 RAG 知识问答（self-check-rag）

基于 **纠错式 RAG（Corrective RAG）** 思路的多阶段知识问答系统：文档检索后先给相关性打分，不合格就自动改写查询或联网补搜，再生成答案，比普通 RAG 更准。

## 功能特点

- 智能文档检索：基于 Qdrant 向量库
- 相关性打分：对检索结果逐条评估，过滤无关内容
- 查询改写：命中不佳时自动优化查询语句
- 联网兜底：本地文档不够时用 Tavily 联网搜索
- 多模型协作：OpenAI 嵌入 + Claude 生成
- Streamlit 交互界面：上传文档即可问答

## 运行方式

```bash
pip install -r requirements.txt
streamlit run self_check_rag.py
```

按提示在界面或环境变量中配置：

- OpenAI API Key（文档嵌入）
- Anthropic API Key（Claude，生成答案）
- Tavily API Key（联网搜索兜底）
- Qdrant Cloud 地址与 API Key（向量库）

> 本项目仅供个人学习与技术交流使用（开源）。代码基于开源项目二次开发，遵循原项目对应的开源协议（Apache-2.0 / MIT），原始项目署名予以保留。
