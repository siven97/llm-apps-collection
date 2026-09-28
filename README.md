# AI Agents 学习合集（AI Agents Collection）

> 本合集仅供个人学习与技术交流使用（开源）。基于开源项目二次开发，遵循原项目对应开源协议，原始署名保留。

一组开箱即用的 LLM / Agent 应用示例，覆盖 **RAG、多智能体、行程规划、网页采集、语音客服、生成式仪表盘** 等方向，每个子目录都是独立可运行的小项目。

## 📦 项目清单

| 目录 | 中文名 | 简介 |
|------|--------|------|
| `self-check-rag/` | 自校验 RAG 知识问答 | 纠错式 RAG：检索后先打分，不行就改写查询或联网补搜 |
| `smart-trip-planner/` | 智能行程规划助手 | 输入目的地/天数/预算，AI 生成行程，可导出日历文件 |
| `model-council/` | 多模型议事会 | 多模型并行回答 + 聚合择优，比单模型更稳 |
| `smart-crawler/` | 智能网页采集器 | 自然语言描述需求即可爬取结构化数据，可本地运行 |
| `voice-desk/` | 语音客服助手 | 基于知识库的语音客服，回答 + TTS 播报 |
| `chart-chat-studio/` | 对话式图表工作台 | 聊天生成实时图表/指标的 Next.js 仪表盘（生成式 UI） |

## 🚀 通用运行说明

- Python 项目（前 5 个）：
  ```bash
  cd <项目目录>
  pip install -r requirements.txt
  streamlit run <主程序>.py
  ```
  API Key 在页面输入框或 `.env` 中配置即可（详见各项目 README）。
- Next.js 项目（`chart-chat-studio/`）：
  ```bash
  cd chart-chat-studio
  pnpm install
  cp .env.example .env   # 填入 GOOGLE_API_KEY
  pnpm dev
  ```

## 🙏 开源归属 / Attribution

- 主体基于 [awesome-llm-apps](https://github.com/Shubhamsaboo/awesome-llm-apps)（Apache-2.0）。
- `chart-chat-studio/` 底层组件基于 [ai-dashboard-canvas-agent](https://github.com/ataibarkai/ai-agents)（MIT，© Atai Barkai）。

> 本合集仅供个人学习与技术交流使用（开源），遵循原项目对应的开源协议。详见根目录 `NOTICE` 与各子目录 `LICENSE`。
