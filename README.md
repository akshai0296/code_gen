```text
coder_debugger/
│
├── src/                      # All core source code
│   ├── generator/            # Code generation logic (e.g., prompt formatting, sampling)
│   │   └── generator.py
│   ├── executor/             # Runtime execution module
│   │   └── executor.py
│   ├── debugger/             # Self-debugging and repair logic
│   │   └── debugger.py
│   ├── coordinator/          # Orchestrates full pipeline (gen → exec → debug)
│   │   └── pipeline.py
│   └── __init__.py           # Makes the code importable
│
├── scripts/                  # Standalone runnable scripts
│   ├── run_pipeline.py       # End-to-end run (single example)
│   ├── batch_eval.py         # Evaluate over DebugBench or MBPP
│   └── train_lora.py         # PEFT (LoRA) fine-tuning script
│
├── benchmarks/               # DebugBench test set + evaluation outputs
│   ├── debugbench.jsonl      # Eval data
│   ├── results/              # Output from model runs
│   └── metrics/              # Accuracy, pass@1, etc.
│
├── notebooks/                # Colab/Jupyter demos
│   └── demo_pipeline.ipynb
└── .gitattributes            # Git LFS tracking
```

Pipeline + QLoRA fine-tuned model that generates, executes, and self-debugs code in Python/Java/C++
