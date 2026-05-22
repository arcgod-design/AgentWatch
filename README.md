
# AgentWatch

> Catch what your AI agent breaks — before it breaks production.

AgentWatch sits between your AI agent and the world. It watches every 
action, scores every reasoning step, blocks dangerous commands, and 
gives you a full replay of exactly what went wrong and why.

No more silent failures. No more "the agent said it succeeded."

---

## The Problem

Your AI agent just deleted the wrong folder. Or worse — it succeeded, 
returned a confident response, and you found out three hours later when 
nothing worked.

Current agents don't tell you when they're about to do something 
dangerous. They don't tell you their confidence is dropping. They don't 
let you roll back. They just run.

AgentWatch fixes that.

---

## What It Does

| | |
|---|---|
| 🛡️ **Safety Engine** | Blocks dangerous commands before they execute |
| 🔍 **Reasoning Auditor** | Scores every reasoning step, not just the final output |
| 📊 **Live Dashboard** | Real-time trace of every action your agent takes |
| ⏪ **One-Click Rollback** | Git-backed checkpoints at every step |
| 🧠 **Persistent Memory** | Your agent remembers context across sessions |
| 💰 **Cost Tracker** | Know exactly what each task costs before it finishes |
| 🔌 **Works With Everything** | Claude Code, LangChain, AutoGPT, any agent |

---

## Quick Start

```bash
pip install agentwatch
docker compose up -d
```

Dashboard → http://localhost:3000  
API → http://localhost:8000

---

## How It Works

AgentWatch wraps your existing agent. You don't rewrite anything.

```python
from agentwatch.adapters.langchain import AgentWatchCallbackHandler

handler = AgentWatchCallbackHandler()
agent_executor = AgentExecutor(agent=..., callbacks=[handler])
```

Every tool call, every reasoning step, every output — captured, scored, 
and available in the dashboard in real time.

---

## Built For The 2026 Agent Problem

76% of AI agent deployments fail within 90 days. Not because the models 
are bad. Because nobody can see what the agent is doing until it's 
already done something irreversible.

AgentWatch is the layer that was missing.

---

## Supported Agents

- Claude Code
- LangChain  
- AutoGPT
- OpenClaw
- Any agent via the Universal Event Schema

---

## License

Apache 2.0
```

