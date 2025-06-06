coder_debugger/
│
├─ src/                  # all importable Python packages
│   ├─ generator/
│   ├─ executor/
│   ├─ debugger/
│   └─ coordinator/
│
├─ benchmarks/           # DebugBench subset, eval scripts, result JSON
├─ notebooks/            # exploratory Colab / Jupyter demos
├─ scripts/              # CLI entry-points, data/download helpers
├─ models/               # empty; checkpoints tracked via Git LFS
├─ docs/                 # MkDocs or Sphinx sources (optional now)
├─ paper/                # final PDF + conference poster
│
├─ requirements.txt
├─ environment.yml       # conda alternative (cuda, bitsandbytes, etc.)
├─ README.md
├─ CONTRIBUTING.md
├─ .gitignore
└─ .gitattributes        # enable Git LFS for *.bin, *.safetensors

# code_gen
Pipeline + QLoRA fine-tuned model that generates, executes, and self-debugs code in Python/Java/C++
