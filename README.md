<p align="center">
  <img src="https://raw.githubusercontent.com/EMT5320/EMT5320/main/assets/profile-header.svg" alt="余凯琪，评测驱动的 LLM Agent 系统工程师" width="100%">
</p>

<p align="center">
  <a href="mailto:1908937833@qq.com">Email</a> ·
  <a href="https://github.com/EMT5320?tab=repositories">全部仓库</a>
</p>

## 我做什么

在某国央企安全事业部做大模型算法与 AI 工程，主导和参与 15+ 个 AI 服务落地生产。多 Agent 研判系统跑到 20+ 专业 Agent、单链路 240+ 次工具调用之后，上下文膨胀、工具预算、证据一致性这些问题都真实出现过。我的做法是把它们拆成可运行、可评测的对照实验，验证过的方法再回到生产架构里。

下面的个人项目各自回答其中一个工程问题。

## Selected Systems

| 项目 | 工程问题 | 关键证据 |
|---|---|---|
| **[AlgoCoach-Flywheel](https://github.com/EMT5320/algocoach-flywheel)** | 代码辅导的「教得好」能否像判题一样被执行验证？ | 42 道 runner-ready 公开题 · 冻结 15 题 / 440 例评测基准 · provenance split 与泄漏审计 · 7B SFT/DPO 全链路 |
| **[ContextGuard Agent Lab](https://github.com/EMT5320/ContextGuard-Agent-Lab)** | 任务、工具、预算固定时，四种 Agent 策略在哪一步分叉？ | 17 cases × 4 strategies = 68 次受控运行 · 独立 grader · FastMCP 工具边界 |
| **[Loomstead](https://github.com/EMT5320/loomstead)** | Agent 的每个动作能否回溯到动机、记忆与工具证据？ | Godot + Python runtime · `phase2.trace` · counterfactual replay · audit packet |
| **[Tsukumo](https://github.com/EMT5320/tsukumo)** | Agent 状态如何跨 runtime 交接，并保留来源、作用域与撤销语义？ | Rust 5-crate workspace · receipt-first · 只读 re-entry · v0.1.0 · Linux/Windows CI |

**Serving / LLMOps：** [LLM Inference Lab](https://github.com/EMT5320/llm-inference-lab) — OpenAI-compatible endpoint benchmark，QPS / TPS / TTFT / P50 / P95，结果按 `historical / live / pending` evidence class 分账保存。

## 技术栈

- **Agent 系统：** 任务规划与多工具调用、多 Agent 编排、LangChain / LangGraph、上下文工程、RAG / MCP、状态交接与 Trace / Replay
- **评测与后训练：** PyTorch / Transformers / PEFT、QLoRA SFT / DPO、DeepSpeed 分布式训练、benchmark 与 grader、数据治理、泄漏审计与人工校准
- **推理与工程：** Python / Rust、vLLM / SGLang、FastAPI、Kafka、SQLite / SQLAlchemy、OpenAI-compatible API、SSE / WebSocket

## 求职方向

**LLM Agent 系统工程 / 大模型评测与后训练 / AI 应用工程** · [1908937833@qq.com](mailto:1908937833@qq.com)
