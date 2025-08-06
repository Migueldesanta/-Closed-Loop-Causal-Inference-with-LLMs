# -Closed-Loop-Causal-Inference-with-LLMs
This repository supports a research project exploring closed-loop causal inference in political science using large language models (LLMs). The framework tests whether a single LLM—or modular prompt-based system—can autonomously execute three stages of a causal experiment: treatment generation, (optional) response simulation, and causal reasoning, all without human-labeled data.

 Framework Overview
Treatment Generation
The LLM generates political message variants (e.g. different framings, tones, or ideological slants) on topics like immigration or surveillance.

(Optional) Simulated Response
The LLM simulates synthetic responses—such as Likert ratings or textual commentary—by different voter types.

Causal Reasoning
Prompted to evaluate whether treatment variations likely caused observed or simulated response differences, the LLM applies counterfactual and confounder logic to infer causal effects.

You may implement the pipeline using a single LLM instance with role-specific prompts, or use separate fine-tuned modules for each stage.

📚 Related Literature & Projects
Ma (2025) and Yu et al. (2024) provide theoretical foundations on LLMs’ capacity for causal inference 
arXiv
Wikipedia
+1
.

Sgouritsa et al. (2024) propose PC-SubQ, a prompting method guiding LLMs step-by-step through a causal discovery algorithm 
arXiv
.

ALCM (Khatibi et al., 2024) integrates data-driven causal discovery with LLM-based refinement 
Benjamin Manning
+15
arXiv
+15
GitHub
+15
.

Manning et al. (2024) present a model using structural causal models and LLMs to generate and test social science hypotheses in silico 
Benjamin Manning
+2
NBER
+2
.

On GitHub, repositories like py-why/pywhyllm demonstrate integrating LLMs into causal analysis pipelines 
ACL Anthology
+15
GitHub
+15
GitHub
+15
.

✨ Key Contributions
End‑to‑End Automated Causal Pipeline: LLM handles design, response simulation (if used), and causal inference in one loop.

Prompt‑Based Modularity: Easily adapt treatment‑creation, response, and reasoning prompts to new topics or political contexts.

Streamlined Hypothesis Generation: Enables early‑stage, cost‑efficient causal hypothesis exploration without labeled survey data.

Extension of Causal Evaluation: Moves beyond causal paraphrases to deeper causal logic use in LLM reasoning.

🚀 Example Applications
Evaluating whether security vs. liberty framing increases public support for surveillance laws

Testing causal impact of populist vs. technocratic messaging on voter attitudes

Generating causal explanations or counterfactual chains in political behavior reasoning
