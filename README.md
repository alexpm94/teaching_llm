# GenAI C1 Project: Teach an LLM to Reason

This project guides you through teaching an instruction-tuned LLM to reason step‑by‑step using GRPO (Group Relative Policy Optimization). The model learns to break a word into letters and count a specific letter.

Key notebooks and files:
- `gen_ai_fundamentals_project_starter.ipynb`
- `requirements_colab_L4.txt`

## Hardware

- The validated Colab run used an `A100`.
- An `L4` ran out of memory for this workflow.
- `requirements_colab_L4.txt` is still the correct dependency file on `A100`.

## Run In Google Colab

1. Open [gen_ai_fundamentals_project_starter.ipynb](/Users/mi23237/cursos/udacity/genai_fundamentals/teaching_llm/gen_ai_fundamentals_project_starter.ipynb) in Google Colab.
2. Set `Runtime -> Change runtime type -> GPU` and choose `A100` if available.
3. Add a Colab secret named `GITHUB_TOKEN`.
4. Run the notebook top to bottom.

The notebook clones the repo, installs from `requirements_colab_L4.txt`, trains the model, and saves the LoRA adapter.

Notes:

- The `GITHUB_TOKEN` secret is used by the clone cell.
- If you only have `L4` and hit OOM, reduce the memory-related model settings or switch runtimes.
- The first `unsloth` import can take a few minutes, and the long training cell can take around an hour.

