---
name: CoEvoskill
description: >
  CoEvoSkills — self-evolving agent skill framework via co-evolutionary
  verification. Lets LLM agents autonomously construct complex, multi-file
  skill packages without ground-truth supervision. Uses a Skill Generator
  and Surrogate Verifier that co-evolve through iterative generate–verify–refine
  cycles. Includes SkillsBench benchmark for evaluation.
  Use this skill to understand, run, or extend the CoEvoSkills framework.
agent_created: true
---

# CoEvoSkills

**CoEvoSkills** is a self-evolving framework that lets LLM agents autonomously construct complex, multi-file skill packages — no ground-truth supervision required.

## Key Ideas

- **Skill Generator** — iteratively produces and refines structured multi-file skill bundles
- **Surrogate Verifier** — information-isolated; independently evolves test assertions to provide dense, actionable failure feedback *without* access to ground-truth test content
- **Ground-truth oracle** — returns only an opaque pass/fail signal, triggering test escalation and preserving information isolation

## Co-Evolution Loop

```
[Skill Generator] ──generates──> [Skill Bundle]
        ↑                               ↓
        └──refines── [Surrogate Verifier] ──feedback──┘
                            ↓
                   [Ground-Truth Oracle] → pass/fail only
```

## What is a Skill?

A skill is a structured, multi-file package with instructions, scripts, and assets — distinct from a single-function tool. CoEvoSkills focuses on generating these complex skill packages automatically.

## SkillsBench

CoEvoSkills includes **SkillsBench**, a benchmark for evaluating skill generation quality across diverse professional tasks.

## References

- GitHub: https://github.com/zhang-henry/CoEvoSkills
- Paper: https://arxiv.org/abs/2604.01687
- Project page: https://zhang-henry.github.io/CoEvoSkills/
