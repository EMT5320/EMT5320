<p align="center">
  <img src="https://raw.githubusercontent.com/EMT5320/EMT5320/main/assets/profile-header.svg" alt="余凯琪，评测驱动的 LLM Agent 系统工程师" width="100%">
</p>

> **把生产 Agent 的复杂问题拆成可运行、可评测的系统。**<br>
> *Building LLM agent systems with execution-grounded evaluation.*

<p align="center">
  <a href="mailto:1908937833@qq.com">Email</a> ·
  <a href="https://github.com/EMT5320?tab=repositories">全部仓库</a>
</p>

## 关于我

人工智能硕士，现从事大模型算法与 AI 工程。工作里把多 Agent、异步服务和本地推理落进真实业务。个人项目把生产中反复出现的问题拆成可运行、可对照的实验。

我主要做 Agent 的任务规划与工具调用，也处理长链路中的上下文和状态。Trace、grader 与 verifier 用来定位失败发生在哪一层。

## 代表项目

### [AlgoCoach-Flywheel](https://github.com/EMT5320/algocoach-flywheel)

把代码辅导的“教得好”转成可执行评测，并连接数据治理与 7B SFT / DPO。<br>
`42 runner-ready problems` · `15 problems / 440 cases` · `protocol split` · 人工校准

### [ContextGuard Agent Lab](https://github.com/EMT5320/ContextGuard-Agent-Lab)

固定任务、工具和预算，比较四种 Agent 策略在哪一步分叉。<br>
`17 cases × 4 strategies` · 独立 grader · FastMCP tool boundary

### [Loomstead](https://github.com/EMT5320/loomstead)

从 Agent 动作回溯到动机、记忆与工具证据，并做 counterfactual replay。<br>
Godot + Python runtime · `phase2.trace` · eval / replay / audit artifacts

### [Tsukumo](https://github.com/EMT5320/tsukumo)

让 Claude / Codex 间的本地状态交接保留来源、作用域与撤销语义。<br>
Rust 5-crate workspace · receipt-first · v0.1.0 · Linux / Windows CI

**模型服务与压测：** [LLM Inference Lab](https://github.com/EMT5320/llm-inference-lab) 是 OpenAI-compatible endpoint benchmark，记录 QPS / TPS / TTFT / P50 / P95，并按 evidence class 分开保存结果。

## 技术栈

- **Agent 系统：** 任务规划与多工具调用、多 Agent 编排、上下文工程、RAG / MCP、状态交接与 Trace / Replay
- **评测与后训练：** PyTorch / Transformers / PEFT、QLoRA SFT / DPO、benchmark 与 grader、数据治理、泄漏审计与人工校准
- **工程与服务：** Python / Rust、FastAPI、Kafka、SQLite / SQLAlchemy、vLLM、OpenAI-compatible API、SSE / WebSocket

## 求职方向与联系

**LLM Agent 系统工程 / 大模型评测与后训练 / AI 应用工程**<br>
[1908937833@qq.com](mailto:1908937833@qq.com)
