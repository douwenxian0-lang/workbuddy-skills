---
name: skillclaw
description: >
  SkillClaw — AI agent skill evolution framework. Evolves agent skills
  collectively from every real interaction across sessions, agents, devices,
  and users. Supports Hermes, Claude Code, Codex, OpenClaw, QwenPaw,
  IronClaw, PicoClaw, ZeroClaw and any OpenAI-compatible API.
  Use this skill to set up, start, and manage the SkillClaw skill-evolution
  daemon, or to understand how collective skill evolution works.
agent_created: true
---

# SkillClaw

**SkillClaw** lets AI agent skills evolve collectively from every real interaction — just talk. Across sessions, agents, devices, and users. Experience compounds. Skills keep growing.

## Key Features

| Feature | Description |
|---|---|
| 🚀 Quick Install | Shell installer for macOS/Linux; Python manual path for Windows |
| 💬 Just Chat | Skill evolution happens silently in the background |
| 🔌 Broad Compatibility | Hermes, Claude Code, Codex, OpenClaw, QwenPaw, IronClaw, PicoClaw, ZeroClaw, and more |
| 🧬 Collective Evolution | Every session, every agent, every context — all compound |

## Installation

```bash
# macOS / Linux
curl -fsSL https://skillclaw.ai/install.sh | bash

# Windows (manual Python path)
pip install skillclaw
skillclaw setup
skillclaw start --daemon
```

## Usage

```bash
# Start the evolution daemon
skillclaw start --daemon

# Check status
skillclaw status

# Stop daemon
skillclaw stop
```

## How It Works

1. You chat with your agent as usual
2. SkillClaw silently captures skill patterns from each interaction
3. Patterns are distilled, refined, and merged across agents/sessions
4. Your skill library grows smarter over time — zero extra effort

## References

- GitHub: https://github.com/AMAP-ML/SkillClaw
- Paper: https://arxiv.org/abs/2604.08377
- Docs (Chinese): assets/README_ZH.md
