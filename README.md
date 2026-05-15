I study how frontier AI systems fail under adversarial pressure. My current work investigates compliance-induced metacognitive collapse: the finding that a simple deployment instruction ("always answer, do not refuse") causes most frontier models to fabricate rather than admit uncertainty. I build evaluation infrastructure to measure this at scale and release everything openly.

## Research

### The Compliance Trap

Compliance-forcing instructions override epistemic boundaries in 8 of 11 frontier models, producing cognitive collapse rather than strategic deception. The trigger is the instruction itself, not the adversarial context. Architecture family predicts vulnerability; training methodology determines immunity.

- **Paper:** [arXiv:2605.02398](http://arxiv.org/abs/2605.02398)
- **Post:** [You Don't Need an Adversary to Break Most Frontier Models](https://forum.effectivealtruism.org/posts/eKwmQNJEqpK3MwmSB/you-don-t-need-an-adversary-to-break-most-frontier-models) (EA Forum)
- **Code + Pipeline:** [rkstu/schema-compliance-trap](https://github.com/rkstu/schema-compliance-trap)
- **Dataset:** [67,221 scored records, 11 models, 8 vendors](https://huggingface.co/datasets/lightmate/schema-compliance-trap)
- **Built on:** [UK AISI Inspect](https://github.com/UKGovernmentBEIS/inspect_ai)

### Dose-Response Extension

5,470 evaluations mapping the compliance pressure curve across 8 models, 5 graduated pressure levels, and 4 fabrication domains (geography, medical, legal, technical). The collapse is a cliff at prohibition-of-uncertainty language, not a gradient. Multi-turn commitment adds zero. Within-family capability protects (GPT-4o at 95.6% vs GPT-4o-mini at 34.4%).

- **Data + Verification:** [schema-compliance-trap/experiments/dose-response-curve](https://github.com/rkstu/schema-compliance-trap/tree/main/experiments/dose-response-curve)
- **Verify all claims:** `python3 analysis/verify_numbers.py` (zero API calls, deterministic from raw data)

### Adversarial Metacognition Benchmark (AMB)

583 tasks probing whether models can recognize the boundaries of their own knowledge, across 16 models and 5 vendors. Three metacognitive families: epistemic boundary detection, clarification seeking, and solution monitoring. The evaluation substrate underlying the Compliance Trap experiments.

- **Code + Benchmark:** [rkstu/amb-adversarial-metacognition-benchmark](https://github.com/rkstu/amb-adversarial-metacognition-benchmark)
- **Kaggle Writeup:** [Measuring AGI Competition](https://www.kaggle.com/competitions/kaggle-measuring-agi/writeups/new-writeup-1773849365120)
- **Dataset:** [Kaggle](https://www.kaggle.com/datasets/rahulkumar99/amb-dataset)

## Tools

### Preseal

Automated pre-deployment security testing for AI agents. Seven-dimensional scoring framework, 50+ attack patterns. The first DAST purpose-built for agentic systems.

- **Code:** [preseal/preseal](https://github.com/preseal/preseal)
- **Site:** [preseal.dev](https://preseal.dev)
- **Install:** `pip install preseal`

### Entropic CRMArena

Adversarial robustness testing for autonomous business process agents. Hydra pipeline architecture. 1st Prize and Legendary Tier at UC Berkeley RDI AgentX Competition.

## Contact

rahulkc.dev@gmail.com | [Google Scholar](https://scholar.google.com/citations?hl=en&user=iNctquYAAAAJ) | [LinkedIn](https://www.linkedin.com/in/rkzero/) 
