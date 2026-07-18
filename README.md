<p align="center">
  <img src="https://raw.githubusercontent.com/EMT5320/EMT5320/main/assets/profile-header.svg" alt="余凯琪，评测驱动的 LLM Agent 系统工程师" width="100%">
</p>

<p align="center">
  <strong>生产 Agent 系统</strong> · <strong>Agent 评测与后训练</strong> · <strong>Trace / Replay</strong> · <strong>Rust Agent Runtime</strong>
</p>

<p align="center">
  <a href="mailto:1908937833@qq.com">Email</a> ·
  <a href="https://github.com/EMT5320?tab=repositories">Repositories</a>
</p>

## 现在聚焦什么

把生产复杂度抽象成可控实验，用 execution receipt、独立 grader、
counterfactual replay 与 claim boundary 测量 Agent 行为，再让证据反向推动
系统架构和后训练决策。

| Agent 系统工程 | 评测 / 后训练 |
|---|---|
| Tool boundary、状态持有、权限与交接 | Protocol split、独立评分、success–cost trade-off |
| Trace、receipt、replay、failure analysis | Verifier-backed data、SFT/DPO、construct validity |
| Python / FastAPI / Kafka / SQLite / Rust | vLLM / OpenAI-compatible endpoints / benchmark governance |

## Selected systems

| System | Engineering question | Evidence receipt | Start here |
|---|---|---|---|
| **AlgoCoach-Flywheel** | 如何把真实练习、可执行验证、数据治理、评测和后训练连成闭环？ | 15 problems / 440 cases；14/20 executed repair；DPO CI 跨 0 | [pipeline + CPU smoke](https://github.com/EMT5320/algocoach-flywheel) |
| **ContextGuard Agent Lab** | 同任务与工具下，不同 Agent 控制策略会在哪里分化？ | 17 cases / 68 runs；独立 grader；四类 strategy split | [case cards + JSONL](https://github.com/EMT5320/ContextGuard-Agent-Lab) |
| **Loomstead** | 如何把复杂 Agent 行为变成可追溯、可 replay 的工程证据？ | trace coverage 1.0；100 LLM evidence records；audit 10/10 | [behavior observatory](https://github.com/EMT5320/loomstead) |
| **Tsukumo** | Agent 状态如何跨 runtime 可信交接，同时保留来源、作用域和撤销语义？ | 5-crate Rust workspace；receipt-first；v0.1.0；Linux/Windows CI | [actual TUI + demo](https://github.com/EMT5320/tsukumo) |

**Serving / LLMOps 邻接证据：** [LLM Inference Lab](https://github.com/EMT5320/llm-inference-lab)
以 endpoint registry、QPS/TPS/P50/P95/TTFT 和 `historical/live/pending`
分账补充模型服务与压测能力；仅在对应 JD 下替换进入主项目组合。

## Working contract

```text
production complexity
  -> controlled experiment
  -> execution-grounded evidence
  -> architecture / policy evolution
```

- 公开项目只写可运行、可回溯的事实；数字必须能回到 report、trace 或 artifact。
- 明确区分 production pattern、bounded benchmark、historical import 与 owner rerun。
- 工程目标是让 Agent 的行为、状态和决策边界可解释、可复验、可撤销。

<sub>Open to evaluation-driven LLM Agent systems, AI developer tools, and model evaluation / post-training roles.</sub>
