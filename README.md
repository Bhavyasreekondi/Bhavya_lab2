# DATA 266 Lab 2

This repository contains the executed notebooks and evaluation materials for DATA 266 Lab 2.

## Repository layout

```text
data266-lab2-teamXX/
├── README.md
├── requirements.txt
├── notebooks/
│   ├── p1_rag.ipynb
│   ├── p2_finetune.ipynb
│   └── p3_agents.ipynb
├── eval/
├── traces/
├── src/
├── CONTRIBUTIONS.md
├── AI_USAGE.md
└── .gitignore
```

## How to run

### Part 1: Multimodal RAG

Open `notebooks/p1_rag.ipynb` in Colab or Kaggle, enable a GPU, upload the provided Part 1 inputs, and run all cells from the beginning. The notebook creates and validates `submission.csv`. Do not commit the PDFs, datasets, or generated extraction files.

### Part 2: Diffusion fine-tuning

Open `notebooks/p2_finetune.ipynb` with a GPU runtime. Run the setup, LoRA configuration, training, generation, evaluation, safety-review, and model-card sections. Store model weights and generated-image artifacts in the designated Hugging Face repository rather than committing them here.

### Part 3: Multimodal multi-agent system

Open `notebooks/p3_agents.ipynb` with a GPU runtime. Run the workflow, normal-scenario evaluation, red-team evaluation, critique-loop comparison, system-card, and Gradio sections. JSON traces may be placed in `traces/` when they do not contain secrets or private data.

## Reproducibility

Install the pinned dependencies with:

```bash
pip install -r requirements.txt
```

Do not commit API keys, Hugging Face tokens, Kaggle credentials, PDFs, datasets, generated image folders, model checkpoints, or runtime caches.

## Submission checklist

- Execute all three notebooks and save their outputs.
- Validate the Part 1 Kaggle `submission.csv`.
- Add the final evaluation files under `eval/`.
- Add non-sensitive Part 3 traces under `traces/`.
- Complete `CONTRIBUTIONS.md` and `AI_USAGE.md`.
- Create Git tags `p1-v1.0`, `p2-v1.0`, and `p3-v1.0` after final verification.
