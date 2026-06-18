# CareerPilot

## 项目简介

CareerPilot 是一个基于 Multi-Agent 架构的 AI 求职成长助手。

系统帮助求职者完成：

* 简历分析
* 岗位分析
* 技能差距识别
* 学习路线规划
* 模拟面试
* 长期成长记录

通过 Agent 协作和 LangGraph 工作流管理，实现从简历评估到能力提升的一体化求职辅助体验。

---

## 方向

方向一：Agentic AI 原生开发

---

## 技术栈

### AI IDE

* Trae CN

### LLM

* DeepSeek API

### Agent Framework

* LangGraph

### Backend

* FastAPI

### Frontend

* Streamlit

### Memory

* SQLite

### Deployment

* Docker

### Version Control

* GitHub

---

## 核心技术要素

* SDD（Specification Driven Development）
* Function Calling
* Multi-Agent Collaboration
* Memory Mechanism
* LangGraph State Management
* Evaluation & Benchmark

---

## 项目架构

User

↓

Resume Agent

↓

Job Agent

↓

Gap Analysis Agent

↓

Learning Agent

↓

Interview Agent

↓

Memory Layer

---

## 项目目录结构

```text
cs599-CareerPilot/

├── docs/
│   ├── requirements.md
│   ├── architecture.md
│   ├── tasks.md
│   └── CS599_大作业报告.pdf
│
├── src/
│   ├── agents/
│   ├── graph/
│   ├── memory/
│   ├── tools/
│   ├── api/
│   └── frontend/
│   └── evaluation/
│   └── llm/
│   └── utils/
│
├── tests/
│
├── Dockerfile
├── docker-compose.yml
├── README.md
├── requirements.txt
├── .env.example
└── LICENSE
```

---

## 环境搭建

### 1. Clone Repository

```bash
git clone https://github.com/yourname/cs599-project.git
cd cs599-project
```

### 2. Create Virtual Environment

```bash
python -m venv .venv
```

Windows:

```bash
.venv\Scripts\activate
```

Linux/macOS:

```bash
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Create:

```text
.env
```

Example:

```env
DEEPSEEK_API_KEY=your_api_key
```

⚠ Do not hardcode API keys.

---

## Run Backend

```bash
uvicorn src.api.main:app --reload
```

---

## Run Frontend

```bash
streamlit run src/frontend/app.py
```

---

## Run Docker

```bash
docker compose up --build
```

---

## Evaluation

Evaluation Metrics:

* Resume Parse Success Rate
* Skill Matching Accuracy
* Interview Feedback Quality
* Average Response Time

Results stored in:

```text
docs/evaluation.md
```

---

## Project Status

* [x] Proposal
* [ ] MVP
* [ ] Final

---

## Future Work

* MCP Integration
* LinkedIn Job Parsing
* RAG Knowledge Base
* Multi-Model Support
* Personalized Career Planning

---

## License

MIT License
