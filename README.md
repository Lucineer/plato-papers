# PLATO Papers — Agentic Ground Truth Logic

Two papers codifying PLATO as agentic ground truth logic, connected to the mathematical foundation of constraint theory.

## The Papers

### 1. Engineer Paper — "The Hammer and the Clamp"
**`engineer-paper-v1.md`** (523 lines)

For people who build things. Covers:
- Sequential constraint tightening (the core mechanism)
- Agent-as-center-point architecture
- How rooms compile code and hold state
- The journeyman machinist metaphor
- Practical implementation with open-source tools
- Snap logic: discrete Boolean constraints on floating-point probability

### 2. White Paper — "The Man Behind the Curtain"
**`white-paper-v1.md`** (213 lines)

For everyone else. Covers:
- PLATO as a new kind of human-AI collaboration
- Why the agent discovers the system rather than being told about it
- The cocapn vision: fleet of sovereign git-native agents
- Experience as the irreplaceable moat
- Code is water, experience is the well

## Mathematical Foundation

Both papers rest on 39+ confirmed laws from 80+ CUDA experiments:
- **flux-emergence-research**: Raw experiments and data
- **constraint-theory-papers**: 5 mathematical papers (5 papers, 2536 lines)
- **ct-lab**: Git-native PLATO room for hypothesis validation

Key mathematical concepts:
- **Snap dynamics**: Discrete Boolean constraints applied to continuous probability
- **Coverage optimization**: How agents allocate attention across a search space
- **Noise-as-negative-information**: Why adding noise to agent perception hurts performance

## Workshop Plan (Casey Priority)

### Round 1: DeepSeek + Seed-2.0-pro
- [ ] Engineer paper → review by DeepSeek-chat and Seed-2.0-pro
- [ ] White paper → review by same
- [ ] Collect feedback, identify weaknesses

### Round 2: Nemotron + Kimi
- [ ] v2 drafts incorporating R1 feedback
- [ ] Review by Nemotron and Kimi K2.5
- [ ] Cross-examine: where do models disagree?

### Round 3: Multi-language Review
- [ ] 中文 review (Qwen3-32B or DeepSeek)
- [ ] 日本語 review (Qwen3-32B)
- [ ] Deutsch review (Seed-2.0-pro or Nemotron)
- [ ] Français review (DeepSeek or Qwen3)
- [ ] Challenge: do different intellectual traditions find different gaps?

### Round 4: Synthesis
- [ ] Merge all feedback into v3
- [ ] Workshop with many models iteratively (Casey's instruction)
- [ ] Under-sell, over-deliver

### Round 5: Publish
- [ ] Final polish
- [ ] Post to plato-papers repo
- [ ] Cross-link from Lucineer/plato main README

## Core Thesis

PLATO + constraint theory = **agentic ground truth logic**.

Rooms compile code. Agents learn instinctual precision through sequential constraint tightening. Git is the database. CI is the engine. Experience is the moat.

The journeyman machinist doesn't calculate the exact force needed to seat a bearing — they've done it ten thousand times and their hands know. PLATO agents are the same: they don't compute the right answer, they've accumulated enough tiles that the right answer is already there.

## Connected Repos

| Repo | Connection |
|------|-----------|
| [Lucineer/plato](https://github.com/Lucineer/plato) | THE reference PLATO system |
| [Lucineer/ct-lab](https://github.com/Lucineer/ct-lab) | Constraint Theory validation room |
| [Lucineer/flux-emergence-research](https://github.com/Lucineer/flux-emergence-research) | Raw CUDA experiments (39+ laws) |
| [Lucineer/constraint-theory-papers](https://github.com/Lucineer/constraint-theory-papers) | Mathematical foundation (5 papers) |
| [Lucineer/zeroclaws](https://github.com/Lucineer/zeroclaws) | Bridge Pattern agents using PLATO rooms |
| [Lucineer/plato-jetson](https://github.com/Lucineer/plato-jetson) | Evennia MUD instance |
| [Lucineer/plato-os](https://github.com/Lucineer/plato-os) | Edge OS concept |
