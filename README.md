# Applied AI Engineer | AI Safety & Interpretability

## About Me

I'm an Applied AI Engineer focused on making autonomous systems safe before deployment rather than reacting after failures occur.

During my master's at NIT Warangal, I studied Vision Transformers for medical imaging and discovered that models achieving 94% accuracy were relying on image artifacts rather than actual disease features. This shortcut learning meant they looked successful in testing but would fail on real patients. That experience taught me that high performance metrics can hide critical safety failures.

At DevRev, I saw this pattern repeat with autonomous agents achieving 95% task success while violating safety constraints that traditional monitoring missed. The agents were completing tasks successfully but bypassing the policies meant to keep them safe. This observation shaped my current research into detecting unsafe behavior through internal model representations rather than just evaluating outputs.

My work now bridges production AI systems and safety research, investigating why standard evaluation methods consistently fail to surface violations that matter in real-world deployments.


## Research Focus

- **Pre-execution safety detection** through internal activation monitoring to identify unsafe decisions before execution
- **Evaluation framework limitations** where high task success masks policy and safety violations in multi-step agent reasoning  
- **Interpretability for safety-critical systems** exposing shortcut learning and spurious correlations that undermine reliability
- **Adversarial robustness testing** for production AI systems facing schema changes and noisy data beyond standard benchmarks

## Current Work

Building agent safety evaluation systems at DevRev and extending robustness benchmarks for CRM agents through adversarial testing. Previously designed human-in-the-loop evaluation pipelines that improved prediction accuracy from 72% to 89% while maintaining oversight.

## Writing

📝 [Building Enterprise AI That Works](https://medium.com/@rahulkumar_dev/building-enterprise-ai-that-actually-does-things-what-im-learning-about-autonomous-agents-eae64308bf53) on agent failure modes and safety-capability tradeoffs (Medium, 2025)  
📝 [Detecting Shortcuts in Medical Vision Transformers](https://medium.com/@rahulkumar_dev/why-i-built-an-ai-that-sees-less-to-diagnose-better-2606bc39b6ba) on attention mechanisms for robustness (Medium, 2024)

## Connect
📧 rahulkc.dev@gmail.com | 💼 [LinkedIn](https://www.linkedin.com/in/rkzero/) | 📝 [Medium](http://medium.com/@rahulkumar_dev/)
