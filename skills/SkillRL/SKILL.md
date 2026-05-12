---
name: SkillRL
description: >
  SkillRL — recursive skill-augmented reinforcement learning framework for
  LLM agents. Transforms successful trajectories into reusable strategic
  patterns and failed ones into concise lessons. Maintains a hierarchical
  SKILLBANK (General Skills + Task-Specific Skills) that co-evolves with the
  agent's policy during RL training. Achieves 10-20% token compression vs
  raw trajectory storage. Evaluated on ALFWorld, WebShop, and Search tasks.
  Use this skill to understand, set up, or extend the SkillRL training pipeline.
agent_created: true
---

# SkillRL

**SkillRL** enables LLM agents to learn high-level, reusable behavioral patterns from past experiences via recursive skill-augmented reinforcement learning.

## Key Features

| Feature | Description |
|---|---|
| 🧠 Skill Distillation | Transforms trajectories into strategic patterns and failure lessons |
| 📚 Hierarchical SKILLBANK | General Skills (universal) + Task-Specific Skills (category-level) |
| 🔄 Recursive Evolution | Skill library co-evolves with agent policy during RL training |
| ⚡ Token Efficiency | 10-20% compression vs raw trajectory storage |

## Supported Tasks

- **ALFWorld** — household task planning
- **WebShop** — web product search & purchase
- **Search** — information retrieval

## Model Checkpoints

| Task | Model | Link |
|---|---|---|
| ALFWorld | SFT | [HuggingFace](https://huggingface.co/Jianwen/Alfworld-7B-SFT) |
| ALFWorld | RL | [HuggingFace](https://huggingface.co/Jianwen/Alfworld-7B-RL) |
| WebShop | SFT | [HuggingFace](https://huggingface.co/Jianwen/Webshop-7B-SFT) |
| WebShop | RL | [HuggingFace](https://huggingface.co/Jianwen/Webshop-7B-RL) |
| Search | SFT | [HuggingFace](https://huggingface.co/Jianwen/Search-7B-SFT) |
| Search | RL | [HuggingFace](https://huggingface.co/Jianwen/Search-7B-RL) |

## Quick Start

```bash
# Install dependencies
pip install -e .

# Generate SFT data
cd examples/sft_data_generation/
python generate.py

# Run RL training (requires verl)
cd recipe/
bash run_skillrl.sh
```

## Directory Structure

```
SkillRL/
├── agent_system/       # Core agent and skill system
├── examples/           # SFT data generation examples
├── recipe/             # Training recipes and configs
├── tests/              # Test suite
├── verl/               # RL training framework (verl)
├── gigpo/              # GigPO algorithm
└── skill_generation/   # Skill generation utilities
```

## References

- GitHub: https://github.com/aiming-lab/SkillRL
- Paper: https://arxiv.org/abs/2602.08234
- SFT Dataset: https://huggingface.co/datasets/Jianwen/SkillRL-SFT-Data
