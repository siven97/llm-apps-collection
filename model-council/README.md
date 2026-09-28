# 多模型议事会（model-council）

多个大模型并行回答同一个问题，再由一个聚合模型挑选 / 融合最优答案（Mixture-of-Agents 思路），比单一模型回答更全面、更稳定。

## 功能特点

- 多模型并行作答，互相补位
- 聚合模型择优融合，输出更稳的最终答案
- Streamlit 界面，API Key 在页面输入即可

## 运行方式

```bash
pip install -r requirements.txt
streamlit run model_council.py
```

在页面输入 Together / OpenAI 等任意 OpenAI 兼容端点的 API Key 即可运行。

> 本项目仅供个人学习与技术交流使用（开源）。代码基于开源项目二次开发，遵循原项目对应的开源协议（Apache-2.0 / MIT），原始项目署名予以保留。
