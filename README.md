<p align="center">
  <img src="https://raw.githubusercontent.com/EMT5320/EMT5320/main/assets/profile-header.svg" alt="余凯琪，评测驱动的 LLM Agent 系统工程师" width="100%">
</p>

<p align="center">
  <a href="mailto:1908937833@qq.com">Email</a>
</p>

## 生产经验

目前在某运营商安全研发团队做大模型算法与 AI 工程，主导和参与 15+ 个 AI 服务上线。SOC 多 Agent 研判系统扩展到 20+ 专业 Agent，代表性链路包含 240+ 次工具调用。系统规模上来后，上下文膨胀、工具预算和证据一致性成了最常处理的问题。我把这类问题拆成可运行的实验，确认边界后再把结果带回生产系统。

## 个人项目

| 项目 | 解决的问题 | 实现与结果 |
|---|---|---|
| **[AlgoCoach-Flywheel](https://github.com/EMT5320/algocoach-flywheel)** | 代码辅导的「教得好」能否像判题一样被执行验证？ | 42 道 runner-ready 公开题 · 冻结 15 题 / 440 例评测基准 · provenance split 与泄漏审计 · 7B QLoRA SFT/DPO served eval 驱动 SFT 基线选择，并将增益与回归切片转入 regression mining |
| **[ContextGuard Agent Lab](https://github.com/EMT5320/ContextGuard-Agent-Lab)** | 任务、工具、预算固定时，四种 Agent 策略在哪一步分叉？ | 16 scored cases × 4 strategies = 64 次受控运行 · 独立 grader · FastMCP 工具边界 |
| **[Loomstead](https://github.com/EMT5320/loomstead)** | Agent 的每个动作能否回溯到动机、记忆与工具证据？ | Godot + Python runtime · `phase2.trace` · counterfactual replay · audit packet |
| **[Tsukumo](https://github.com/EMT5320/tsukumo)** | Agent 状态如何跨 runtime 交接，并保留来源、作用域与撤销语义？ | Rust 5-crate workspace · receipt-first · 只读 re-entry · v0.1.0 · Linux/Windows CI |

**推理服务：** [LLM Inference Lab](https://github.com/EMT5320/llm-inference-lab)，面向 OpenAI-compatible endpoint 对比 QPS / TPS / TTFT 和延迟分位数，并区分历史压测导入与现场复跑。

## 技术栈

- **Agent 系统：** 任务规划与 Tool Use / Function Calling、多 Agent 编排、LangChain / LangGraph、上下文工程、RAG / MCP、状态交接与 Trace / Replay
- **评测与后训练：** PyTorch / Hugging Face Transformers / PEFT、QLoRA SFT / DPO、benchmark、自动化 grader 与 LLM-as-a-Judge、训练 / 评测数据构建与治理、泄漏审计与人工校准
- **推理与工程：** Python、FastAPI / Pydantic、vLLM 多卡部署、OpenAI-compatible API、KV Cache / 长上下文与并发调优、Kafka、SSE / WebSocket

## 求职方向

**LLM Agent 系统工程 / 大模型评测与后训练 / AI 应用工程** · [1908937833@qq.com](mailto:1908937833@qq.com)
