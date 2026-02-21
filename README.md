# Building deep understanding of Neural Networks

The deep implementation work **Andrej Karpathy's Zero to Hero neural network series** — arguably the best free resource for going from zero to a genuine understanding of how modern deep learning works. Karpathy is a rare force in this field: someone at the frontier of AI research who also cares deeply about making that knowledge accessible to everyone. That he releases material of this quality for free is something worth being genuinely grateful for.

---

## How I'm Learning

### How to Watch

Every video gets **two passes**:

- **First pass:** Watch straight through. No notes, no pausing. Build the mental scaffold.
- **Second pass:** Notebook + Jupyter open. Pause constantly. Write concepts in my own words. Type all code yourself. Break things. Try things.

The second pass is currently taking me 6x longer than the video. That's the point.

### How I Build the Notebooks

**Every line of code is typed by hand.** No copy-pasting from the video or the repo. The friction of typing forces you to actually think about what each line does — and the bugs you inevitably introduce teach you more than the correct code would.

The notebooks are also built to read like explanations — as if I were teaching the material to someone else. This isn't just a documentation choice; it's a learning strategy. The act of explaining something clearly forces you to find the gaps in your own understanding and fill them. If I can't write a precise explanation of why something works, I don't actually understand it yet.

---

## Citations

The core implementation work in this repository follows:

> Karpathy, A. (2022). _Neural Networks: Zero to Hero_ [Video series]. YouTube.
> https://karpathy.ai/zero-to-hero.html

Intuition-building follows:

> Sanderson, G. (3Blue1Brown). (2017–2024). _Neural networks_ [Video series]. YouTube.
> https://www.youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi

---

## License

MIT License

Copyright (c) 2025 Kshitij

Permission is hereby granted, free of charge, to any person obtaining a copy of this repository and associated documentation files, to deal in the repository without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the materials, and to permit persons to whom the repository is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the materials.

THE MATERIALS ARE PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE MATERIALS OR THE USE OR OTHER DEALINGS IN THE MATERIALS.

> **Note:** The original lecture content, code, and videos are the work of Andrej Karpathy and 3Blue1Brown. This repository contains only personal notes, explanations, and derivative educational work created while following their material. Please refer to their original repositories and channels for the authoritative source.

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
