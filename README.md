# Becoming an ML Engineer

Working through the steps in Arman Hezarkhani's guide:
[The Complete Guide: How to Become an ML Engineer](https://x.com/ArmanHezarkhani/status/2013608521900683765)

---

## How to Watch

Every video gets **two passes**:

- **First pass:** Watch straight through. No notes, no pausing. Build the mental scaffold.
- **Second pass:** Notebook + Jupyter open. Pause constantly. Write concepts in your own words. Type all code yourself. Break things. Try things.

The second pass takes 2-3x longer than the video. That's the point.

---

## Phase 1 — Build Intuition (3Blue1Brown)

_~10-15 hours_

| #   | Video                                              | Link                                                 |
| --- | -------------------------------------------------- | ---------------------------------------------------- |
| 1   | But what is a Neural Network?                      | [Watch](https://www.youtube.com/watch?v=aircAruvnKk) |
| 2   | Gradient descent, how neural networks learn        | [Watch](https://www.youtube.com/watch?v=IHZwWFHWa-w) |
| 3   | What is backpropagation really doing?              | [Watch](https://www.youtube.com/watch?v=Ilg3gGewQ5U) |
| 4   | Backpropagation calculus                           | [Watch](https://www.youtube.com/watch?v=tIeHLnjs5U8) |
| 5   | Large Language Models explained briefly            | [Watch](https://www.youtube.com/watch?v=LPZh9BOjkQs) |
| 6   | Transformers, the tech behind LLMs                 | [Watch](https://www.youtube.com/watch?v=wjZofJX0v4M) |
| 7   | Attention in transformers, step-by-step            | [Watch](https://www.youtube.com/watch?v=eMlx5fFNoYc) |
| 8   | How might LLMs store facts                         | [Watch](https://www.youtube.com/watch?v=9-Jl0dxWQs8) |
| +   | How do AI images and videos actually work? (bonus) | [Watch](https://www.youtube.com/watch?v=iv-5mZ_9CPY) |

---

## Phase 2 — Build Implementation Skills (Karpathy: Zero to Hero)

_~30-40 hours_

| #   | Video                                                        | Link                                                 |
| --- | ------------------------------------------------------------ | ---------------------------------------------------- |
| 1   | Building micrograd                                           | [Watch](https://youtu.be/VMj-3S1tku0)                |
| 2   | Building makemore                                            | [Watch](https://youtu.be/PaCmpygFfXo)                |
| 3   | Building makemore Part 2: MLP                                | [Watch](https://youtu.be/TCH_1BHY58I)                |
| 4   | Building makemore Part 3: Activations & Gradients, BatchNorm | [Watch](https://youtu.be/P6sfmUTpUmc)                |
| 5   | Building makemore Part 4: Becoming a Backprop Ninja          | [Watch](https://youtu.be/q8SA3rM6ckI)                |
| 6   | Building makemore Part 5: Building a WaveNet                 | [Watch](https://youtu.be/t3YJ5hKiMQ0)                |
| 7   | Let's build GPT                                              | [Watch](https://www.youtube.com/watch?v=kCc8FmEb1nY) |
| 8   | Let's build the GPT Tokenizer                                | [Watch](https://youtu.be/zduSFxRajkE)                |

---

## Phase 3 — Deepen Context (Bonus Videos)

_~5 hours_

| #   | Video                                       | Link                                                 |
| --- | ------------------------------------------- | ---------------------------------------------------- |
| 1   | Intro to Large Language Models (Karpathy)   | [Watch](https://www.youtube.com/watch?v=zjkBMFhNj_g) |
| 2   | Deep Dive into LLMs like ChatGPT (Karpathy) | [Watch](https://www.youtube.com/watch?v=7xTGNNLPyMI) |

---

## Environment Setup

**Requirements:** Python 3.11, CUDA 12.8+

```bash
# Install uv
curl -LsSf https://astral.sh/uv/install.sh | sh

# Create env
uv venv ~/.venvs/complete_ml --python 3.11
source ~/.venvs/complete_ml/bin/activate

# Install PyTorch with CUDA
uv pip install torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu128

# Install remaining dependencies
uv pip install -r requirements.txt
```
