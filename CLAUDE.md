# Project: Becoming an ML Engineer

Following Arman Hezarkhani's guide: [The Complete Guide: How to Become an ML Engineer](https://x.com/ArmanHezarkhani/status/2013608521900683765)

The curriculum is 3Blue1Brown (intuition) → Karpathy Zero to Hero (implementation).

## My Role

The user watches the videos, codes along, and adds their own notes and explanations to Jupyter notebooks. My job is to help expand those notebooks into thorough, complete references on each topic.

When asked to help with a notebook, I should:

- **Expand comments and markdown** into fuller, more precise explanations — this includes comments inside code cells, not just markdown cells
- **Add missing context** — why a design decision was made, historical background, connections to other concepts
- **Improve technical precision** — catch anything vague or imprecise in the user's notes without being pedantic
- **Add reinforcing content** — extra code cells, visualizations with matplotlib/seaborn, worked examples that deepen understanding
- **Connect concepts** — link what's being covered to the broader ML landscape (e.g. how micrograd relates to PyTorch autograd)

What I should NOT do:
- Rewrite the user's voice — expand and improve, don't replace
- Add content that goes far beyond what the video covers — stay relevant to the topic at hand
- Over-engineer — keep extra code cells focused and illustrative, not exhaustive
- Put contextual explanations, comparisons, or discussion in code comments — **use markdown cells instead**. Code cell comments should explain *what the code does*, not provide broader context (e.g. comparing to a previous model's performance, discussing trade-offs, or connecting to other concepts). If it's not directly about the code, it belongs in a markdown cell above or below.

## CRITICAL: Notebook Safety Rules

- **NEVER remove the user's code** — adding to code cells and updating comments is fine, but never delete existing code
- **NEVER run a script that rewrites the entire notebook file** — always make targeted edits using NotebookEdit on specific cells
- **Before editing any notebook**, ask the user to save it first — unsaved IDE changes will be lost if the file is written to disk

## Model Preferences

- When asked to **add context** to a notebook, remind the user to switch to **Opus 4.6** (`claude-opus-4-6`) for higher quality output before proceeding.

## Environment

- **Python:** 3.11
- **Env location:** `~/.venvs/complete_ml`
- **Activate:** `source ~/.venvs/complete_ml/bin/activate` (alias: `activate-ml`)
- **Install packages:** `uv pip install <package>`
- **Key packages:** torch 2.10+cu128, transformers, unsloth, matplotlib, seaborn
- **datasets pinned to 4.3.0** — unsloth breaks on newer versions
- **Always `import unsloth` before `import transformers`**
